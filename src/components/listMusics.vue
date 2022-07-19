<template>
  <div>
    <h2>music lists</h2>
    <songElement />
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
