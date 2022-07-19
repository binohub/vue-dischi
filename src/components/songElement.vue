<template>
  <div id="songElement">

    <div class="card bg-dark">

      <img class="card-img-top" :src="song.poster"
        alt="song">
      <div class="card-body d-flex flex-column align-items-center justify-content-center">
        <h5 class="card-title">{{ song.title }}</h5>
        <p class="card-text card-artist"> {{song.author}} </p>
        <p class="card-text card-year">{{song.year}}</p>
      </div>

    </div>

  </div>
</template>

<script>
export default {
  props: ["song"],
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#songElement {
  color: white;
  padding: 2rem;

  .card-title {
    font-weight: bold;
    font-size: 1rem;
    text-align: center;
  }

  .card-text {
    color: lightgray;
    font-weight: bold;
    font-size: .5rem;
  }
}
</style>
