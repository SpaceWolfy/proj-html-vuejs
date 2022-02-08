<template>
  <div id="app">
    <div v-if="!isLoading">
      <loading-screen />
    </div>
    <div v-else>
      <header-box :headerNav="headerNav" />
      <main-section />
      <footer-box />
    </div>
  </div>
</template>

<script>
import HeaderBox from "./components/HeaderBox.vue";
import MainSection from "./components/MainSection.vue";
import FooterBox from "./components/FooterBox.vue";
import LoadingScreen from "./components/LoadingScreen.vue";

export default {
  name: "App",
  components: { HeaderBox, MainSection, FooterBox, LoadingScreen },
  data() {
    return {
      //array semplice - TODO: trasformazione in array di oggetti con link di collegamento alle sezioni del sito
      headerNav: ["Home", "About Us", "Feature", "Testimonials", "Contact US"],
      isLoading: false,
    };
  },
  mounted() {
    setTimeout(() => (this.isLoading = true), 3000);
  },
};
</script>

<style lang="scss">
@import "@/style/Main.scss";
#app {
  margin: 0 auto;
  width: 1250px;
}
</style>
