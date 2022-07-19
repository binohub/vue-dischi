<template>
  <div id="listMusics">

    <div class="container">
      <div class="row">
        <div class="col-3">
          <songElement />
        </div>
      </div>
    </div>


  </div>
</template>

<script>
import songElement from './songElement.vue';

export default {
  components: {
    songElement,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
