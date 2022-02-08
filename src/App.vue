<template>
  <div id="app">
    <div v-if="!isLoading">
      <loading-screen />
    </div>
    <div v-else>
      <header-box :headerNav="headerNav" />
      <main-section :boxArray="boxArray" />
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
      /* headerNav: ["Home", "About Us", "Feature", "Testimonials", "Contact US"], */
      headerNav: [
        {
          voice: "Home",
          href: "#app",
        },

        {
          voice: "About us",
          href: "#about-us",
        },
        {
          voice: "Feature",
          href: "#features",
        },
        {
          voice: "Testimonials",
          href: "#testimonials",
        },
        {
          voice: "Contact US",
          href: "#contacts",
        },
      ],

      boxArray: [
        {
          title: "Customized Invoices",
          image: require("./assets/icons/chart-ico.jpg"),
        },

        {
          title: "Stock Management",
          image: require("./assets/icons/plane-ico.jpg"),
        },
        {
          title: "Receivable & Payables",
          image: require("./assets/icons/medal-ico.jpg"),
        },
        {
          title: "Manage Buying",
          image: require("./assets/icons/person-ico.jpg"),
        },
        {
          title: "Powerful & Secure",
          image: require("./assets/icons/intersection-ico.jpg"),
        },
        {
          title: "Fastest Return Filing",
          image: require("./assets/icons/medal-ico.jpg"),
        },
        {
          title: "Monthly Detailed",
          image: require("./assets/icons/exam-ico.jpg"),
        },
        {
          title: "Product Management",
          image: require("./assets/icons/like-ico.jpg"),
        },
      ],
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
  width: 1400px;
}
</style>
