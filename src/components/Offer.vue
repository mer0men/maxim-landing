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
    <button class="btn">ЗАПИСАТЬСЯ</button>
  </div>
</template>

<style lang="scss" scoped>
.offer {
  height: 100vh;
  background: url("../assets/1bg.jpg") 100% auto;
  position: relative;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;

  .info {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 64px 0;
    width: 50%;

    span {
      text-transform: uppercase;
      font-size: 36px;
      line-height: 46px;
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
      width: 80%;
      border: 1px solid #e52600;
    }

    .head {
      font-size: 64px !important;
      line-height: 81px !important;
    }

    p {
      margin: 0;
      padding: 0;
      font-size: 30px;
      line-height: 38px;
    }
  }

  p {
    font-size: 24px;
    line-height: 30px;
  }
}
</style>
