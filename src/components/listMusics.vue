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
import axios from 'axios';

export default {
  data: function(){
    return{

    }
  },
  components: {
    songElement,
  },
  methods:{
    getSong(){
      //recupero i personaggi
      console.log("recupera i personaggi");
      axios.get("")
      .then((result) => {
        console.log(result);
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
