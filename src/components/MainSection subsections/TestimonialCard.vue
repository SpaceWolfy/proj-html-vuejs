<template>
  <div class="container">
    <div class="carousel">
      <div class="carousel-item" v-show="toggle">
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
      </div>

      <div class="carousel-item" v-show="!toggle">
        <div class="card-container">
          <div
            class="card"
            v-for="(person, index) in testimonialsP2"
            :key="index"
          >
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
      </div>

      <div class="carousel-nav">
        <div class="dot-box">
          <div
            class="dot"
            @click="toggle = !toggle"
            :class="{ selected: toggle }"
          ></div>
          <div
            class="dot"
            @click="toggle = !toggle"
            :class="{ selected: !toggle }"
          ></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return { toggle: true };
  },
  props: {
    testimonial: Array,
    testimonialsP2: Array,
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
@import "@/style/MainS-Components/TestimonialCard.scss";
</style>
