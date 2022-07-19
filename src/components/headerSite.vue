<template>
  <header class="d-flex align-items-center"> 
    
    <div class="uwuContainer">
      <nav class="navbar navbar-dark bg-dark">
        <a class="navbar-brand" href="#">
          <img src="../assets/img/Spotify_logo_without_text.svg.png" width="50" height="50" alt="">
        </a>
      </nav>
    </div>
    
  </header>
</template>

<script>
export default {
  name: 'headerSite',
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  background-color: #212529;
  height: 10vh;
}
</style>
