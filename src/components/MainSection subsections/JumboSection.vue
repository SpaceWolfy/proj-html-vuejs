<template>
  <div class="main">
    <div class="left-side">
      <div class="text">
        <div class="title">The biggest platform for your growth.</div>
        <p>
          There are many variations of passages of Lorem Ipsum available, but
          the majority have suffered alteration in some form
        </p>
      </div>
      <button class="general-btn">Read More</button>
    </div>

    <div class="right-side">
      <img src="../../assets/img/27-1.png" alt="" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/style/Variables.scss";
@import "@/style/Utility.scss";

.main {
  background-color: #f2f7ff;
  display: flex;
  height: 500px;
  padding: 0 35px 0 70px;
  border-radius: 10px;

  .left-side {
    padding-top: 50px;
    .title {
      line-height: 80px;
      font-size: 52px;
      margin-bottom: 30px;
    }

    p {
      color: #8e989f;
      font-size: 17px;
      line-height: 30px;
      margin-bottom: 50px;
    }
  }

  .right-side {
    padding-top: 20px;
    img {
      width: 750px;
    }
  }
}
</style>
