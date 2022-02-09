<template>
  <div class="container" id="testimonials">
    <div class="card-container">
      <div class="card" v-for="(person, index) in testimonial" :key="index">
        <img :src="person.image" alt="" />

        <div class="text">
          <div class="name">
            {{ person.personName }}
            - <span class="role">{{ person.role }}</span>
          </div>

          <p>{{ person.description }}</p>
        </div>

        <div class="little-border"></div>
        <div class="mini-border"></div>
      </div>
    </div>
    <div class="dot-box">
      <div class="dot"></div>
      <div class="dot"></div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    testimonial: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/MainS-Components/TestimonialCard.scss";
</style>
