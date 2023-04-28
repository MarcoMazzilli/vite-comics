<script>
import "../components/film-card/Card.vue"
import CardVue from './film-card/Card.vue'
import arrayFilm from "../data/dc-comics.json"

export default {
data(){
    return{
      arrayFilm,
    }
  },  
  components:{
    CardVue,
  }
}
</script>

<template>

  <div class="main-wrapper">
    <div class="container">
      
      <CardVue 
      v-for="(film , index) in arrayFilm" :key="index" 
      :img="film.thumb"
      :text="film.series"
      />
      
    </div>
  </div>


</template>


<style lang="scss" scoped>
@use "../../src/scss/partials/vars" as * ;

.main-wrapper{
  min-height: $main-height;
  background-color: $bg-main;

  .container{
    min-height: $main-height;
    padding-top: 60px;
    color: white;
    display: flex;
    flex-wrap: wrap;
  }
}

</style>