<script>
import CtaSection            from './components/Cta-section.vue';
import Footer                from './components/Footer.vue';
import Header                from './components/Header.vue';
import Main                  from './components/Main.vue';
import SocialFooterSection   from './components/Social-footer-section.vue';
import Jumbotron             from './components/Jumbotron.vue';

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
    CtaSection,
    SocialFooterSection,
    Jumbotron,
}
}
</script>
<!-- /SCRIPT -->

<!-- TEMPLATE -->
<template>
  
  <Header />

  <Jumbotron />
    
  <Main />

  <Cta-section />
  
  <Footer />

  <SocialFooterSection />
  
</template>
<!-- /TEMPLATE -->

<!-- STYLE -->
<style lang="scss">
@import "./scss/main.scss";

</style>
<!-- /STYLE -->