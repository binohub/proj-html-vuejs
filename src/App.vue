<template>
  <div id="app">
      <headerSite />
      <mainSite />
      <footerSite />

  </div>
</template>

<script>
import headerSite from './components/headerSite.vue'
import mainSite from './components/mainSite.vue'
import footerSite from './components/footerSite.vue'

export default {
  name: 'App',
  components: {
    headerSite,
    mainSite,
    footerSite,
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
@import "bootstrap-icons/font/bootstrap-icons.css";
@import "./assets/style/var.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
