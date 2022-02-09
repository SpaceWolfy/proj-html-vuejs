<template>
  <div class="wave-bg">
    <img src="../../assets/img/15.png" alt="" />
    <div class="main">
      <div class="text">
        <div class="title">Our Testimonials</div>
        <p>
          If you are planning on developing a product landing app or website,
          <br />
          take a look at this beautiful crafted
        </p>
      </div>

      <div class="testimonial-card">
        <testimonial-card :testimonial="testimonials" />
      </div>
    </div>
  </div>
</template>

<script>
import TestimonialCard from "./TestimonialCard.vue";
export default {
  components: { TestimonialCard },
  props: {
    testimonials: Array,
  },
};
</script>

<style lang="scss" scoped>
.wave-bg {
  margin-top: 50px;
  width: 100%;
  height: 800px;

  //fix del gradino fastidioso
  box-shadow: inset 0px 4.5px 0px 0px #fff;

  //gradient
  background: rgb(255, 255, 255);
  background: linear-gradient(
    0deg,
    rgba(255, 255, 255, 1) 30%,
    rgba(242, 247, 255, 1) 100%
  );

  .main {
    margin: 0 auto;
    width: 1400px;

    .text {
      margin-top: -110px;
      text-align: center;
      /* margin-bottom: 50px; */
      .title {
        font-size: 38px;
        margin-bottom: 20px;
      }

      p {
        font-size: 17px;
        line-height: 30px;
      }
    }
  }
}
</style>
