<template>
  <footer>
    <div class="main">
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
@import "@/style/Variables.scss";
footer {
  margin-top: 130px;
  border-top: 1px solid #ebebeb;

  .main {
    display: flex;
    width: 1400px;
    margin: 0 auto;
    padding: 60px 135px;
  }

  .left-side {
    font-size: 16px;
    img {
      width: 140px;
      margin-bottom: 10px;
    }

    p {
      line-height: 28px;
      margin-bottom: 50px;
    }

    .copyright {
      color: #8e989f;
      span {
        color: $blue;
      }
    }
  }

  .right-side {
    display: flex;
    margin-left: 130px;

    .list-container {
      .section-title {
        font-size: 20px;
        color: $darkGrey;
        padding-bottom: 30px;
      }

      ul {
        li {
          color: #8e989f;
          line-height: 40px;
        }
      }
    }

    .list-container:nth-child(2) {
      margin: 0 230px;
    }
  }
}
</style>
