<template>
  <div class="card-container">
    <div class="card" v-for="(post, index) in posts" :key="index">
      <img :src="post.image" alt="" />
      <div class="date">{{ post.date }}</div>

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
@import "@/style/Variables.scss";
.card-container {
  display: flex;
  padding: 0 160px;
  justify-content: space-between;
  .card {
    padding: 10px;
    width: 340px;
    border: 1px solid $border1;
    border-radius: 5px;
    position: relative;

    img {
      width: 100%;
    }

    .date {
      position: absolute;
      color: $grey;
      padding: 5px 10px;
      background-color: white;
      top: 20px;
      left: 20px;
      border-radius: 5px;
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
