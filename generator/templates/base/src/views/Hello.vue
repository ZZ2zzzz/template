<!--
 * @Description: 
 * @Author: my2zzh <leo@easestrategy.com>
 * @Date: 2019-11-08 16:09:04
 * @LastEditTime: 2019-11-08 16:11:35
 * @LastEditors: my2zzh <leo@easestrategy.com>
 -->
<style lang="scss">
</style>

<template>
  <div>
    <p>{{msg}}</p>
    <HelloWorld></HelloWorld>
  </div>
</template>

<script>
import api from '@/api';
import HelloWorld from '@/components/HelloWorld'
export default {
  name: 'hello',
  components: {
    HelloWorld
  },
  data() {
    return {
      msg: 'demo page'
    }
  },
  created() {
    api.login({}).then( res => {

    })
  }
}
</script>
