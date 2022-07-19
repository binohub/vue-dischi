<template>
  <div id="mainSite">

      <listMusics />
    
  </div>
</template>

<script>
import listMusics from './listMusics.vue';

export default {
    components: {
        listMusics,
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

#mainSite{
  padding: 5rem;
  background-color: #1e2d3b;
}
</style>
