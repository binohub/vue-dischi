<template>
  <div id="listMusics">

    <div class="container">
      <div class="row">
          <songElement class="col-3" :song="song"
          v-for="(song, index) in songs" :key="index"/>
      </div>
    </div>


  </div>
</template>

<script>
import songElement from './songElement.vue';
import axios from 'axios';

export default {
  data: function(){
    return{
      songs: [],
    }
  },
  components: {
    songElement,
  },
  methods:{
    getSong(){
      //recupero i personaggi
      console.log("recupera i personaggi");
      axios.get("https://flynn.boolean.careers/exercises/api/array/music")
      .then((result) => {
        this.songs = result.data.response;
        console.log(this.songs);
      })
      .catch((error) => {
        console.warn(error);
      })
    }
  },
  created(){
    this.getSong();
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
