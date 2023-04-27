<script>
import {footerLink} from "../data/menus-db"

export default {
data(){
    return{
      footerLink,
    }
}  
}
</script>

<template>
<div class="main-wrapper">
  <div class="container">
    <!-- TODO: FUNCTION TO AUTO PRINT LINKS -->
    <div class="left">

      <div class="col">
        <ul>
          <h4>DC COMICS</h4>
          <li v-for="(title,index) in footerLink[0].dcComics" :key="index"><a :href="title.url"> {{ title.label }} </a></li>
        </ul>

        <ul>
          <h4>SHOP</h4>
          <li v-for="(title,index) in footerLink[1].shop" :key="index"><a href="#">{{ title.label }}</a></li>

        </ul>

      </div>

      <div class="col">
        <ul>
          <h4>DC</h4>
          <li v-for="(title,index) in footerLink[2].dc" :key="index"><a href="#">{{ title.label }}</a></li>
        </ul>
      </div>

      <div class="col">
        <ul>
          <h4>SITES</h4>
          <li v-for="(title,index) in footerLink[3].sites" :key="index"><a href="#">{{ title.label }}</a></li>
        </ul>
      </div>

    </div>

    <div class="right">
      <img src="../assets/img/dc-logo-bg.png" alt="">
    </div>

  </div>
</div>
</template>

<style lang="scss" scoped>
@use "../../src/scss/partials/vars" as * ;

.main-wrapper{
  height: $footer-height;
  background-image: url(../assets/img/footer-bg.jpg);
  overflow-y: hidden ;

  .container{
    display: flex;
    justify-content: space-between;
    height: 100%;

    .left{
      display: flex;
      width: 50%;
      padding-top: 40px;

      .col{
        width: 25%;

        ul{
          list-style: none;

          h4{
            color: white;
            margin-bottom: 20px;
          }

          li{
            margin: 5px 0;
            &:hover a{
              color: white;
            }

            a{
              color: $main-light-grey;
              text-decoration: none;
              text-transform: capitalize;
            }
          }
        }
      }

      .col:first-child{
        ul:first-child {
          margin-bottom: 30px;
        }
      }
    }

    .right{
      width: 50%;
      position: relative;

      img{
        position: absolute;
        right: 0;
        transform: scale(1.5);
      }
    }
  }
}

</style>