<script>

export default {
    data(){
        return{
        }
    },
    props :{
        img: String,
        text: String
    }
   }
</script>

<template>

      
      <!-- -- -->
      <div class="card">
        <div class="card-img">
          <img :src="img" :alt="text">
        </div>
        <div class="card-description">
          <span>{{ text }}</span>
        </div>
      </div>
      <!-- -- -->

</template>

<style lang="scss" scoped>
@use "../../scss/partials/vars" as *;

    .card{
      width: calc(100%/6);
      padding: 15px;
    }
    .card-img{
      aspect-ratio: 2/3;
      margin-bottom: 15px;
      
      img{
        object-fit: cover;
        object-position: center;
        aspect-ratio: 2/3;
      }
    }
    .card-description{
      span{
        text-transform: uppercase;
      }
    }

</style>