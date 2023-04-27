<script>
export default {
data(){
    return{
      name : "Header"
    }
}  
}
</script>

<template>
  <h1>{{ name }}</h1>
</template>

<style lang="scss" scoped>
@use "../../src/scss/partials/vars" as * ;

h1{
    background-color: $bg-header;
}

</style>