<template>
  <div id="app">
    <header-box />
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
};
</script>

<style lang="scss">
@import "@/style/Main.scss";
#app {
  width: 1250px;
}
</style>
