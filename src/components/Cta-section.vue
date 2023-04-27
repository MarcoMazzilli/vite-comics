<script>
export default {
data(){
    return{
      name : "cta"
    }
}  
}
</script>

<template>
<div class="main-wrapper">
    <div class="container">
        <ul>
            <!-- TODO: AUTOMATIC PRINT FUNCTION -->
            <li>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <p>label img</p>
            </li>
            <li>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <p>label img</p>
            </li>
            <li>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <p>label img</p>
            </li>
            <li>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <p>label img</p>
            </li>
            <li>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <p>label img</p>
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
                
                img{
                    height: 75px;
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