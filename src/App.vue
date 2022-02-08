<template>
  <div id="app">
    <header-box :headerNav="headerNav" />
    <main-section />
    <footer-box />
  </div>
</template>

<script>
import HeaderBox from "./components/HeaderBox.vue";
import MainSection from "./components/MainSection.vue";
import FooterBox from "./components/FooterBox.vue";

export default {
  name: "App",
  components: { HeaderBox, MainSection, FooterBox },
  data() {
    return {
      //array semplice - TODO: trasformazione in array di oggetti con link di collegamento alle sezioni del sito
      headerNav: ["Home", "About Us", "Feature", "Testimonials", "Contact US"],
    };
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
