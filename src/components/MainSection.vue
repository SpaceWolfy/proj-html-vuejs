<template>
  <main>
    <jumbo-section />

    <online-marketing />

    <tip-section />

    <feature-section />

    <testimonials />

    <posts-section />

    <contact-section />
  </main>
</template>

<script>
import ContactSection from "./MainSection subsections/ContactSection.vue";
import FeatureSection from "./MainSection subsections/FeatureSection.vue";
import JumboSection from "./MainSection subsections/JumboSection.vue";
import OnlineMarketing from "./MainSection subsections/OnlineMarketing.vue";
import PostsSection from "./MainSection subsections/PostsSection.vue";
import Testimonials from "./MainSection subsections/Testimonials.vue";
import TipSection from "./MainSection subsections/TipSection.vue";

export default {
  components: {
    JumboSection,
    OnlineMarketing,
    TipSection,
    FeatureSection,
    Testimonials,
    PostsSection,
    ContactSection,
  },
};
</script>

<style lang="scss" scoped></style>
