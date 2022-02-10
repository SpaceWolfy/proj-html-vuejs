<template>
  <main>
    <div class="p-width">
      <jumbo-section />

      <about-us />

      <tip-section />
    </div>

    <feature-section :boxArray="boxArray" />

    <testimonials
      :testimonials="testimonials"
      :testimonialsP2="testimonialsP2"
    />

    <div class="p-width">
      <posts-section :posts="posts" />

      <contact-section />
    </div>
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
    testimonials: Array,
    testimonialsP2: Array,
    posts: Array,
  },
};
</script>

<style lang="scss" scoped></style>
