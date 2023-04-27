<script>
import {headerLink} from "../data/menus-db"
export default {
data(){
    return{
      headerLink,
    }
}
}

</script>

<template>

  <div class="container">

    <img src="../assets/img/dc-logo.png" alt="">

    <ul>
        <li @click="link.active = !link.active" v-for="(link, index) in headerLink" :key="index" :class="{ 'active' : link.active }">
            <a :href="link.url">{{link.label}}</a>
        </li>
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
        &:hover, &.active{
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