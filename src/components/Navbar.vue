<template>
  <div class="navbar">
    <div class="brand">
      <img src="../assets/logo.png" alt="" />
    </div>
    <div class="nav-items">
      <span>о нас</span>
      <span>спикеры</span>
      <span>записаться</span>
    </div>
  </div>
</template>

<style lang="scss">
.navbar {
  position: fixed;
  top: 0;
  width: 100%;
  display: flex;
  justify-content: space-between;
  height: 144px;

  .brand {
    img {
      height: 138px;
      width: 138px;
    }
  }

  .nav-items {
    span {
      text-transform: uppercase;
      margin: 0 16px;
      font-size: 30px;
      line-height: 38px;
    }
  }
}
</style>
