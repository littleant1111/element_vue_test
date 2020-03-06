<template>
  <div id="app" class="sys-app">
    <router-view></router-view>
  </div>
</template>

<script>
  import Cookie from 'js-cookie'
  export default {
    name: 'app',
    components: {
    },
    beforeMount() {
      console.log('beforeMount ...');
    }
  }
</script>

<style>
  @import "assets/css/base.css";
</style>
