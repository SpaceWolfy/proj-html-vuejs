<template>
  <div class="main">
    <div class="left-side">
      <div class="text">
        <div class="title">Get tips tricks on how to skyrocket your sales.</div>
        <p>
          Faff about a quid blower i don't want no agro bleeding chimney pot
          burke tosser cras nice one boot fanny.!
        </p>
      </div>

      <div class="info-container shadowed">
        <div class="info-img">
          <img src="../../assets/img/510.png" alt="" />
        </div>

        <div class="info text">
          <div class="blue par-name">Reporting Analysis</div>
          <p>
            {{ paragraph }}
          </p>
        </div>
      </div>

      <div class="info-container">
        <div class="info-img">
          <img src="../../assets/img/511.png" alt="" />
        </div>

        <div class="info text">
          <div class="par-name grey">Technical SEO Audit</div>
          <p>
            {{ paragraph }}
          </p>
        </div>
      </div>
    </div>

    <div class="right-side">
      <img src="../../assets/img/509.jpeg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      paragraph:
        "It is a long estabilished fact that a reader will be distracted by the readable content of a page when looking at its layout",
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/MainS-Components/TipSection.scss";
</style>
