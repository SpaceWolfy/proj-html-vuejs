<template>
  <div>
    <div class="main" id="features">
      <div class="circle">
        <img src="../../assets/img/14.png" alt="" />
      </div>

      <header>
        <div class="left-side">
          <div class="text">
            <div class="title">Popular features that your business needs</div>
            <p>
              Faff about a quid blower i don't want no agro bleeding chimney pot
              burke tosser cras nice one boot fanny.!
            </p>
          </div>
        </div>

        <div class="right-side">
          <button class="general-btn">Explore More Feature</button>
        </div>
      </header>
      <div class="flex-box">
        <div
          class="box-container"
          v-for="(card, index) in boxArray"
          :key="index"
        >
          <div class="text-cont">{{ card.title }}</div>
          <div class="img-cont"><img :src="card.image" alt="" /></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  props: {
    boxArray: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/MainS-Components/FeatureSection.scss";
</style>
