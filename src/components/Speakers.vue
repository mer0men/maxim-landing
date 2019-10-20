<template>
  <div class="speakers">
    <h2 class="header">СПИКЕРЫ</h2>
    <div class="speakers-box">
      <div class="speaker">
        <img src="../assets/1spk.jpg" alt="" />
        <p class="name">Городняя Дарья</p>
        <hr />
        <p class="info">
          Специалист по продвижению в социальных сетях, агентство
          интернет-маркетинга «Беркана», (г.Владивосток)
        </p>
      </div>
      <div class="speaker main">
        <img src="../assets/2spk.jpg" alt="" />
        <p class="name">Татьяна Зяблицкая</p>
        <hr />
        <p class="info">
          Эксперт по созданию брендов для малого бизнеса , Дальневосточное
          бренд-агентство «Стратегия Успеха».
        </p>
      </div>
      <div class="speaker">
        <img src="../assets/3spk.jpg" alt="" />
        <p class="name">Любавская Наталия</p>
        <hr />
        <p class="info">
          Агентство интернет-маркетинга «Беркана», (г.Владивосток)
        </p>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.speakers {
  position: relative;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-direction: column;

  .header {
    font-size: 64px;
    line-height: 81px;
    color: #e52600;
  }

  .speakers-box {
    display: flex;
    width: 100%;
    justify-content: space-around;
    align-items: center;

    .speaker {
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;

      img {
        width: 400px;
        height: 480px;
      }

      main {
        img {
          transform: scale(1.2);
        }
      }

      .name {
        font-size: 24px;
        line-height: 30px;
      }

      .info {
        font-size: 18px;
        line-height: 23px;
      }

      hr {
        width: 70%;
        border: 2px solid #e52600;
      }
    }
  }
}
</style>
