<template>
  <div class="card-container">
    <div class="card" v-for="(post, index) in posts" :key="index">
      <img :src="post.image" alt="" />

      <div class="text">
        <div class="title">{{ post.title }}</div>
        <p>{{ post.description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    posts: Array,
  },
};
</script>

<style lang="scss" scoped>
.card-container {
  display: flex;
  padding: 0 160px;
  justify-content: space-between;
  .card {
    padding: 10px;
    width: 340px;
    border: 1px solid #eff1fe;
    border-radius: 5px;

    img {
      width: 100%;
    }

    .text {
      margin: 5px 15px;
      .title {
        margin: 28px 0 20px 0;
        font-size: 20px;
      }

      p {
        line-height: 30px;
        width: 85%;
      }
    }
  }
}
</style>
