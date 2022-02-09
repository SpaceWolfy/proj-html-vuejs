<template>
  <div class="card-container">
    <div class="card" v-for="(person, index) in testimonial" :key="index">
      <div class="little-border"></div>
      <div class="mini-border"></div>
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
.card-container {
  margin-top: 100px;
  display: flex;
  justify-content: space-around;
  padding: 0 35px;
  .card {
    height: 300px;
    width: 500px;
    position: relative;
    border-radius: 3px;
    border: 1px solid #000000;

    .little-border,
    .mini-border {
      position: absolute;
      left: 0;
      right: 0;
      margin: auto;
      border-bottom-left-radius: 3px;
      border-bottom-right-radius: 3px;
      border: 1px solid black;
    }

    .little-border {
      bottom: -12px;
      background-color: red;
      height: 12px;
      width: 440px;
    }

    .mini-border {
      bottom: -21px;
      background-color: blueviolet;
      height: 10px;
      width: 410px;
    }
  }
}
</style>
