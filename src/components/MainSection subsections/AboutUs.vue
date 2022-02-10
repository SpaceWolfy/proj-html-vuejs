<template>
  <div class="main" id="about-us">
    <!-- Sezioni identiche, piuttosto che gestirle con un array ho preferito replicarle -->
    <div class="section" v-for="number in 3" :key="number">
      <div class="img-24"><img src="../../assets/img/24.png" alt="" /></div>

      <div class="text">
        <div class="title">Online Marketing</div>
        <p>It is a long estabilished fact that a reader will be distracted</p>

        <ul>
          <li><i class="fas fa-check"></i>SEO</li>
          <li><i class="fas fa-check"></i>SEM</li>
          <li><i class="fas fa-check"></i>Website Strategy</li>
          <li><i class="fas fa-check"></i>Social management</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/style/Variables.scss";
.main {
  margin: 180px 90px;
  display: flex;

  .section {
    display: flex;

    .img-24 {
      margin-right: 30px;
      img {
        width: 80px;
      }
    }

    .text {
      .title {
        font-size: 25px;
      }

      p {
        margin: 20px 0 40px 0;
        width: 85%;
      }

      ul {
        font-size: 15px;
        font-weight: bold;
        li {
          padding-bottom: 20px;

          .fas {
            color: $blue;
            margin-right: 15px;
          }
        }
      }
    }
  }
}
</style>
