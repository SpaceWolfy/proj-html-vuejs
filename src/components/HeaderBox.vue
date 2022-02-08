<template>
  <header>
    <div class="logo"><img src="../assets/img/logo-2.png" alt="" /></div>

    <nav>
      <ul v-for="items in headerNav" :key="items">
        <li>{{ items }}</li>
      </ul>
    </nav>

    <div class="iconFunctions">
      <i class="fas fa-search"></i>
      <i class="fas fa-shopping-cart"></i>
    </div>

    <button class="general-btn">Get Started</button>
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
@import "@/style/Variables.scss";
</style>
