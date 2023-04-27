<script>
import CtaSection from './components/Cta-section.vue';
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
      Footer,
      CtaSection }
}
</script>
<!-- /SCRIPT -->

<!-- TEMPLATE -->
<template>
  
  <Header />
  
  <Main />

  <cta-section />
  
  <Footer />
  
</template>
<!-- /TEMPLATE -->

<!-- STYLE -->
<style lang="scss">
@import "./scss/main.scss";

</style>
<!-- /STYLE -->