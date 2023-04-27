<script>
export default {
data(){
    return{
      message : "--> Content goes Here! <--"
    }
}  
}
</script>

<template>
  <div class="main-wrapper">
    
    <div class="container">
      
      <h1>{{ message }}</h1>
      
    </div>

  </div>
</template>

<style lang="scss" scoped>
@use "../../src/scss/partials/vars" as * ;

.main-wrapper{
  background-color: $bg-main;
  
  .container{
    display: flex;
    align-items: center;
    height: $header-height;
    color: white;
  }

}
</style>