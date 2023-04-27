<script>
import {ctaLinks} from "../data/menus-db"
export default {
data(){
    return{
        ctaLinks,

    }
}  
}
</script>

<template>
<div class="main-wrapper">
    <div class="container">

        <ul>
            <li v-for="(product, index) in ctaLinks" :key="index">
                <img :src=" product.src" :alt="product.src">
                <p>{{ product.label }}</p>
            </li>
        </ul>
    </div>
</div>
</template>

<style lang="scss" scoped>
@use "../../src/scss/partials/vars" as * ;

.main-wrapper {
    background-color: $main-blue;
    height: $cta-section-height ;

    .container{
        height: 100%;
        
        ul{
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: space-around;

            li{
                display: flex;
                align-items: center;
                gap: 15px;
                cursor: pointer;

                &:hover{
                    transform: scale(1.2);
                    transition: .5s;
                }
                
                img{
                    height: 50px;
                }
                p{
                    color: white;
                    text-transform: uppercase;
                }
            }
        }
    }
}

</style>