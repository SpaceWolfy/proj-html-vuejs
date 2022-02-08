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
          <div class="par-name">Technical SEO Audit</div>
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
@import "@/style/Variables.scss";
.main {
  margin: 0 90px;
  display: flex;
  justify-content: space-between;

  .left-side {
    .text {
      width: 510px;
      margin-bottom: 50px;
      .title {
        font-size: 38px;
        margin-bottom: 25px;
      }

      p {
        font-size: 17px;
        line-height: 30px;
      }
    }

    .info-container {
      width: 90%;
      margin: 10px 0;
      padding: 20px;
      display: flex;

      .info-img {
        align-self: center;
      }

      .info {
        margin: 0 15px;
        .par-name {
          font-size: 20px;
          margin-bottom: 15px;
        }

        .blue {
          color: $blue;
        }
      }
    }

    .shadowed {
      border: 1px solid #f0f0f0;
      box-shadow: 2px 30px 20px #f0f0f0;
    }
  }

  .right-side {
    align-self: center;
  }
}
</style>
