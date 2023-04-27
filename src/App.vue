<script>
import Footer from './components/Footer.vue';
import Header from './components/Header.vue';
import Main from './components/Main.vue';

export default {
    data() {
        return {
            name: "Marco"
        };
    },
    components: { 
      Header,
      Main,
      Footer }
}
</script>
<!-- /SCRIPT -->

<!-- TEMPLATE -->
<template>
  
  <Header />
  
  <Main />
  
  <Footer />
  
</template>
<!-- /TEMPLATE -->

<!-- STYLE -->
<style lang="scss">
@import "./scss/main.scss";

</style>
<!-- /STYLE -->