<script>
export default {
data(){
    return{
      name : "Footer"
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
    background-color: $bg-footer;
}

</style>