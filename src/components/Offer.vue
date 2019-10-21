<template>
  <div class="offer">
    <div class="info">
      <span>24 октября</span>
      <span>| 10:00 - 14:00 |</span>
      <span>Владивосток</span>
    </div>
    <div class="header">
      <h1 class="head">ЛИЧНЫЙ БРЕНД – СОЗДАВАЙ И ПРОДВИГАЙ</h1>
      <hr />
      <p>
        Мастер-класс для специалистов, руководителей, экспертов и
        предпринимателей разного уровня
      </p>
    </div>
    <p>“Вам стоит узнать, как это монетизировать!”</p>
    <button class="btn" v-scroll-to="{
        el: '.contacts',
        offset: -50,
        duration: 1100
      }">ЗАПИСАТЬСЯ</button>
  </div>
</template>

<style lang="scss" scoped>
.offer {
  height: 100vh;
  background: url("../assets/1bg.jpg");
  background-size: 100% 100%;
  position: relative;
  display: flex;
  justify-content: center;
  background-repeat: no-repeat;
  flex-direction: column;
  align-items: center;
  width: calc(100% - 112px);
  padding: 24px 56px;


  .info {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 64px 0;
    min-width: 50%;

    span {
      text-transform: uppercase;
      font-size: 30px;
      line-height: 38px;
    }
  }

  .header {
    width: 80%;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    margin: 36px 0;

    hr {
      width: 90%;
      border: 1px solid #e52600;
    }

    .head {
      font-size: 56px !important;
      line-height: 60px !important;
      margin-bottom: 0;
    }

    p {
      margin: 0;
      padding: 0;
      font-size: 24px;
      line-height: 38px;
    }
  }

  p {
    font-size: 20px;
    line-height: 30px;
    margin: 64px 0;
  }
}
</style>
