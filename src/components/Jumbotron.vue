<script>
export default {
data(){
    return{
      message : "--> Jumbotron! <--"
    }
}  
}
</script>

<template>
  <div class="main-wrapper">
    
    <div class="container">
      <div class="current-series">
        <span>current series</span>
      </div>
    </div>

  </div>
</template>

<style lang="scss" scoped>
@use "../scss/partials/vars" as *;

.main-wrapper{
    height: $jumbotron-height;
    position: relative;
    background-image: url(../assets/img/jumbotron.jpg);
    .current-series{
        position: absolute;
        background-color: $main-blue;
        padding: 10px;
        bottom: -25px;

        span{
            color: white;
            font-size: 1.5rem;
            font-weight: 600;
            text-transform: uppercase;
        }
    }
}

</style>