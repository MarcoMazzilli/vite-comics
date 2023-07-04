
<script>
import {footerSocialIcons} from "../data/menus-db"

export default {
    data(){
    return{
      footerSocialIcons,
    }
}  
}
</script>

<template>

<div class="main-wrapper">
    <div class="container">

        <div class="button-container">
            <div id="button">SING-UP NOW!</div>
        </div>

        <div class="social-icons">
            <h3>follow us</h3>
            <ul>
                <li v-for="(src,i) in footerSocialIcons" :key="i"><img :src="src" alt=""></li>
            </ul>
        </div>

    </div>
</div>

</template>

<style lang="scss" scoped>
@use "../scss/partials/vars" as * ;

.main-wrapper{
    height: $footer-social-height;
    background-color: $bg-footer ;

    .container{
        height: 100%;
        display: flex;
        justify-content: space-between;

        .button-container{
            display: flex;
            align-items: center;

            #button{
               border: 2px solid $main-blue; 
               padding: 15px;
               color: white;
               font-weight: bold;
            }
        }

        .social-icons{
            padding: 0 15px;
            display: flex;
            align-items: center;

            h3{
                color: $main-blue;
                text-transform: uppercase;
                margin-right: 25px;
                font-size: 1.5rem;
            }
            ul{
                display: flex;
                list-style: none;
                gap: 20px;

                li{
                    cursor: pointer;
                    &:hover {
                        transform: scale(1.1);
                    }
                }
            }
        }
    }

}

</style>