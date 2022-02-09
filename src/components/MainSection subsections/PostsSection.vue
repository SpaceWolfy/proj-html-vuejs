<template>
  <div class="main">
    <div class="text">
      <div class="title">Latest Posts</div>
      <p>If you are planning on developing a product landing.</p>
    </div>

    <post-card :posts="posts" />
  </div>
</template>

<script>
import PostCard from "./PostCard.vue";
export default {
  components: { PostCard },
  props: {
    posts: Array,
  },
};
</script>

<style lang="scss" scoped>
.main {
  margin-top: 55px;
  .text {
    text-align: center;
    margin-bottom: 110px;
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
</style>
