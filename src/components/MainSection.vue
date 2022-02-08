<template>
  <main>
    <jumbo-section />

    <about-us />

    <tip-section />

    <feature-section :boxArray="boxArray" />

    <testimonials />

    <posts-section />

    <contact-section />
  </main>
</template>

<script>
import ContactSection from "./MainSection subsections/ContactSection.vue";
import FeatureSection from "./MainSection subsections/FeatureSection.vue";
import JumboSection from "./MainSection subsections/JumboSection.vue";
import AboutUs from "./MainSection subsections/AboutUs.vue";
import PostsSection from "./MainSection subsections/PostsSection.vue";
import Testimonials from "./MainSection subsections/Testimonials.vue";
import TipSection from "./MainSection subsections/TipSection.vue";

export default {
  components: {
    JumboSection,
    AboutUs,
    TipSection,
    FeatureSection,
    Testimonials,
    PostsSection,
    ContactSection,
  },
  props: {
    boxArray: Array,
  },
};
</script>

<style lang="scss" scoped></style>
