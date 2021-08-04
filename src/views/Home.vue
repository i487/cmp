<template>
  <div class="home">
    <img src="../assets/intro-back.png" alt="" class="back-img">
    <Header />
    <div class="container">
      <Introsection />     
      <Business-section />
    </div>
    <Cards-section />
    <div class="container">
      <Solution-section />
      <Portfolio />
      <Partners />
      <Consulting-section />
    </div>
    <Strategy />
    <div class="container">
      <Team />
      <Reviews />
      <Contact />
      <Articles />
    </div>
    <Footer />
  </div>
</template>

<script>
import Articles from '../components/Articles.vue';
import BusinessSection from '../components/BusinessSection.vue';
import CardsSection from '../components/CardsSection.vue';
import ConsultingSection from '../components/ConsultingSection.vue';
import Contact from '../components/Contact.vue';
import Footer from '../components/Footer.vue';
import Header from '../components/Header.vue';
import Introsection from '../components/Introsection.vue';
import Partners from '../components/Partners.vue';
import Portfolio from '../components/Portfolio.vue';
import Reviews from '../components/Reviews.vue';
import SolutionSection from '../components/SolutionSection.vue';
import Strategy from '../components/Strategy.vue';
import Team from '../components/Team.vue';

export default {
  components: { Header, Introsection, BusinessSection, CardsSection, SolutionSection, Portfolio, Partners, ConsultingSection, Strategy, Team, Reviews, Contact, Articles, Footer},
  name: "Home",
  
};
</script>

<style lang="scss">
.home {
  .back-img {
        position: absolute;
        right: 0;
        top: 0;
        z-index: -1;
  }
}
</style>

