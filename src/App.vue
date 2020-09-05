<template>
  <div class="app">
    <router-view />
  </div>
</template>

<style lang="scss">
@import './assets/scss/main.scss';

.app {
  height: 100vh;
  width: 100%;
}
</style>

<script>
export default {
  name: 'App'
}
</script>
