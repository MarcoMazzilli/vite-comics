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

  <div class="container">

    <img src="../assets/img/dc-logo.png" alt="">

    <ul>
        <li><a href="#">characters</a></li>
        <li><a href="#">comics</a></li>
        <li><a href="#">movies</a></li>
        <li><a href="#">tv</a></li>
        <li><a href="#">games</a></li>
        <li><a href="#">collectibles</a></li>
        <li><a href="#">videos</a></li>
        <li><a href="#">fans</a></li>
        <li><a href="#">news</a></li>
        <li><a href="#">shop</a></li>

    </ul>
  </div>

</template>

<style lang="scss" scoped>
@use "../../src/scss/partials/vars" as * ;

.container{
    height: $header-height  ;
    display: flex;
    align-items: center;
    justify-content: space-between;

    img{
        height: 85%;
    }
}

ul{
    display: flex;
    list-style: none;
    height: 100%;
    
    li{
        display: flex;
        align-items: center;
        height: 100%;
        border-bottom: 5px solid $bg-header;
        margin: 0 10px;
        
        // TODO: add class active on <li> element
        &:hover{
            border-bottom: 5px solid $main-blue;
            cursor: pointer;
        }
        
        &:hover a {
            color: $main-blue;
        }
        a{
            text-decoration: none;
            text-transform: uppercase;
            font-weight: 600;
            font-size: .9rem;
            color: $main-grey;
        }
    }
}

</style>