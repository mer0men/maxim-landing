<template>
  <div class="navbar">
    <div class="brand">
      <img src="../assets/logo.png" alt="" />
    </div>
    <div class="nav-items">
      <span v-scroll-to="{
        el: '.cases',
        offset: -50,
        duration: 1100
      }">о нас</span>
      <span v-scroll-to="{
        el: '.speakers',
        offset: -50,
        duration: 1100
      }">спикеры</span>
      <span v-scroll-to="{
        el: '.contacts',
        offset: -50,
        duration: 1100
      }">записаться</span>
    </div>
  </div>
</template>

<style lang="scss">
.navbar {
  position: absolute;
  top: 0;
  left: 0;
  width: calc(100% - 48px);
  display: flex;
  justify-content: space-between;
  height: 144px;
  padding: 0 24px;
  z-index: 1000;

  .brand {
    img {
      height: 138px;
      width: 138px;
    }
  }

  .nav-items {
    padding: 16px;

    span {
      text-transform: uppercase;
      margin: 0 16px;
      font-size: 24px;
      line-height: 38px;
      cursor: pointer;
    }
  }
}
</style>
