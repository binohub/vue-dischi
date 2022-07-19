<template>
  <div id="app">
    <headerSite />
    <mainSite />
    <footerSite />
  </div>
</template>

<script>
import headerSite from './components/headerSite.vue';
import mainSite from './components/mainSite.vue';

export default {
  name: 'App',
  components: {
    headerSite,
    mainSite,
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

.uwuContainer {
  width: 80%;
  margin: 0 auto;
  color: white;
}
</style>
