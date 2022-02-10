<template>
  <footer>
    <div class="p-width">
      <div class="left-side">
        <img src=".././assets/img/35.png" alt="" />

        <p>
          It is a long estabilished fact that a <br />
          reader will be distracted by the <br />
          readable content.
        </p>

        <div class="copyright">Copyright @ 2018 <span>Sofbox</span></div>
      </div>
      <div class="right-side">
        <div
          class="list-container"
          v-for="(object, index) in footerNav"
          :key="index"
        >
          <div class="section-title">
            {{ object.section }}
          </div>
          <ul>
            <li v-for="(voice, i) in object.voice" :key="i">{{ voice }}</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="go-up">
      <a href="#home"> <i class="fa-solid fa-angle-up"> </i></a>
    </div>
  </footer>
</template>

<script>
export default {
  props: {
    footerNav: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/FooterBox.scss";
</style>
