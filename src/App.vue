<template>
  <div id="app">
<md-avatar>
  <img src="./assets/avatar-2.jpg" alt="Avatar">
</md-avatar>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
@import "assets/css/reset.css";
</style>
