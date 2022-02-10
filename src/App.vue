<template>
  <div id="app">
    <div v-if="!isLoading">
      <loading-screen />
    </div>
    <div v-else>
      <header-box :headerNav="headerNav" />
      <main-section
        :boxArray="boxArray"
        :testimonials="testimonials"
        :testimonialsP2="testimonialsPageTwo"
        :posts="posts"
      />
      <footer-box :footerNav="footerNav" />
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
      //array(obj) for header
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

      //array(obj) for features section
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

      /* Array(obj) for testimonials carousel */
      testimonials: [
        {
          personName: "Julia Aann",
          image: require("./assets/img/26.jpeg"),
          role: "COO Sofbox",
          description:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip",
        },
        {
          personName: "Mac Znder",
          image: require("./assets/img/27.jpeg"),
          role: "Manager Sofbox",
          description:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip",
        },
      ],

      testimonialsPageTwo: [
        {
          personName: "Cipolletta",
          image: require("./assets/img/25.jpeg"),
          role: "Sofbox Lawyer",
          description:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip",
        },
      ],
      /*  */

      //array(obj) for post section
      posts: [
        {
          title: "Life Lack Meaning",
          image: require("./assets/img/17.jpg"),
          description:
            "It is a long estabilished fact that a reader will be distracted by the readable.",
          date: "November 28, 2019",
        },
        {
          title: "Life Lack Meaning",
          image: require("./assets/img/18.jpg"),
          description:
            "It is a long estabilished fact that a reader will be distracted by the readable.",
          date: "November 28, 2019",
        },
        {
          title: "Life Lack Meaning",
          image: require("./assets/img/19.jpg"),
          description:
            "It is a long estabilished fact that a reader will be distracted by the readable.",
          date: "November 28, 2019",
        },
      ],

      //array(obj) for Footer section
      footerNav: [
        {
          section: "Menu",
          voice: ["About us", "Theme", "Features", "Pricing", "Blog"],
        },
        {
          section: "About Us",
          voice: ["About Sofbox", "Roadmap", "How it works", "Team", "News"],
        },
        {
          section: "Quick Links",
          voice: ["About us", "Theme", "Features", "Pricing", "Blog"],
        },
      ],
      isLoading: false,
    };
  },
  mounted() {
    //Gestisce il tempo di visualizzazione del loading screen
    setTimeout(() => (this.isLoading = true), 3000);
  },
};
</script>

<style lang="scss">
@import "@/style/Main.scss";
</style>
