<template>
  <div id="mainSite">
    <div class="uwuContainer">
      <h1>main</h1>
      <listMusics />
    </div>
    
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
  height: 90vh;
  background-color: #1e2d3b;
}
</style>
