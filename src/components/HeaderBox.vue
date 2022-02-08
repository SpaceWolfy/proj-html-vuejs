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
        <i class="fas fa-shopping-cart"></i>
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
@import "@/style/Variables.scss";
@import "@/style/Utility.scss";

header {
  height: 70px;
  padding-top: 12px;
  display: flex;
  justify-content: space-around;

  .logo {
    width: 45px;
    margin-right: 100px;
    img {
      width: 100%;
    }
  }

  .right-side {
    display: flex;
    align-items: center;

    nav {
      display: flex;
      padding-bottom: 6px;

      ul {
        list-style: none;
        font-size: 17px;
        padding: 17px;

        li {
          padding: 17px 0;
          border-bottom: 2px solid transparent;
          &:hover {
            border-bottom: 2px solid $blue;
          }

          a {
            color: $darkGrey;
          }

          &:hover a {
            color: $blue;
          }
        }
      }
    }

    .icon-functions {
      margin: 35px;

      .fas {
        margin: 15px;

        &:hover {
          color: $blue;
        }
      }
    }
  }
}
</style>
