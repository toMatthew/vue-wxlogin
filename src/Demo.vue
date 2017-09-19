<template>
  <div id="app">
    <div id="wxbox">
      <wxlogin :appid="appid" :scope="scope" :redirect_uri="redirect_uri"></wxlogin>
    </div>
    
  </div>
</template>

<script>
import wxlogin from './components/vue-wxlogin'

export default {
  name: 'app',
  components: {
    wxlogin
  },
  data () {
      return {
          appid : 'wxe1f5def243e0390b',
          scope : 'snsapi_login',
          redirect_uri : 'https://abstest.tenpay.com/abs/author/callBack.do',
      }
  },
}
</script>

<style>
#wxbox{
  width: 400px;
  height: 400px;
}
</style>
