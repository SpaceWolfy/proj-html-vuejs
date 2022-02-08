<template>
  <header>
    <div class="logo"><img src="../assets/img/logo-2.png" alt="" /></div>

    <div class="right-side">
      <nav>
        <ul v-for="items in headerNav" :key="items">
          <li>
            <a href="">{{ items }}</a>
          </li>
        </ul>
      </nav>

      <div class="icon-functions">
        <i class="fas fa-search"></i>
        <i class="fas fa-shopping-cart"><div class="shop-num">0</div></i>
      </div>

      <button class="general-btn">Get Started</button>
    </div>
  </header>
</template>

<script>
export default {
  props: {
    headerNav: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/HeaderBox.scss";
</style>
