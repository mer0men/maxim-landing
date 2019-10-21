<template>
  <div class="contacts">
    <div class="info">
      <span>24 октября</span>
      <span>| 10:00 - 14:00 |</span>
      <span>Партизанский пр-т, 58</span>
    </div>
    <p class="price">Стоимость участия: 4 000 руб.</p>
    <div class="form">
      <input v-model.trim="name" type="text" name="name" placeholder="Ф.И.О." />
      <input
        v-model.trim="email"
        type="text"
        name="email"
        placeholder="E-mail"
      />
      <input
        v-model.trim="number"
        type="text"
        name="number"
        placeholder="Номер телефона"
      />
    </div>
    <button class="btn" @click="send">записаться</button>
    <div class="contact-info">
      <div class="item">
        <svg
          width="25"
          height="25"
          viewBox="0 0 25 25"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M24.9881 19.7263C25.041 20.1321 24.9174 20.485 24.6175 20.7849L21.0976 24.2782C20.9388 24.4547 20.7315 24.6048 20.4757 24.7281C20.2199 24.8517 19.9685 24.9311 19.7216 24.9663C19.7039 24.9663 19.6509 24.9709 19.5626 24.9797C19.4745 24.9885 19.3598 24.993 19.2187 24.993C18.8833 24.993 18.3408 24.9356 17.5909 24.8209C16.841 24.7062 15.9236 24.4238 14.8386 23.974C13.7533 23.5241 12.5227 22.8491 11.1465 21.9494C9.77035 21.0497 8.30587 19.8145 6.75322 18.2442C5.51815 17.0267 4.49481 15.8623 3.68319 14.7507C2.87158 13.6391 2.21875 12.6114 1.72473 11.6674C1.23066 10.7235 0.860136 9.86776 0.613123 9.10026C0.366109 8.33275 0.198493 7.67111 0.110274 7.11533C0.0220548 6.55955 -0.0132329 6.12286 0.00441096 5.80527C0.0220548 5.48768 0.0308767 5.31125 0.0308767 5.27596C0.0661643 5.02894 0.145562 4.77752 0.269068 4.52169C0.392575 4.26585 0.542548 4.05854 0.718986 3.89974L4.23893 0.379798C4.48594 0.132784 4.76824 0.00927734 5.08583 0.00927734C5.3152 0.00927734 5.51811 0.0754417 5.69454 0.20777C5.87098 0.340099 6.02095 0.503304 6.14446 0.697387L8.9763 6.06993C9.13509 6.35223 9.1792 6.661 9.10862 6.99623C9.03805 7.33146 8.88808 7.61377 8.65871 7.84313L7.36189 9.13996C7.3266 9.17524 7.29572 9.23259 7.26925 9.31198C7.24279 9.39138 7.22956 9.45755 7.22956 9.51048C7.30013 9.881 7.45893 10.3044 7.70594 10.7808C7.91767 11.2043 8.24408 11.7204 8.68517 12.3291C9.12627 12.9378 9.75262 13.6391 10.5642 14.4331C11.3582 15.2448 12.064 15.8754 12.6815 16.3254C13.2989 16.7752 13.8152 17.1061 14.2298 17.3179C14.6444 17.5296 14.962 17.6575 15.1825 17.7015L15.5132 17.7677C15.5485 17.7677 15.606 17.7544 15.6853 17.728C15.7647 17.7015 15.8221 17.6707 15.8574 17.6353L17.3659 16.1003C17.6837 15.8181 18.054 15.6769 18.4775 15.6769C18.7775 15.6769 19.0156 15.7298 19.192 15.8357H19.2184L24.3263 18.8528C24.6969 19.0823 24.9174 19.3734 24.9881 19.7263Z"
            fill="#010002"
          />
        </svg>
        <span>8-984-198-28-51</span>
      </div>
      <div class="item">
        <svg
          width="25"
          height="25"
          viewBox="0 0 25 25"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M3.21 0.000976562H21.7915C23.5568 0.000976562 25 1.44464 25 3.20998V21.7915C25 23.5563 23.5568 24.999 21.7915 24.999H3.21C1.44467 24.999 0 23.5562 0 21.7915V3.20998C0 1.44464 1.44467 0.000976562 3.21 0.000976562ZM18.2122 2.77739C17.5923 2.77739 17.0868 3.28498 17.0868 3.90448V6.59731C17.0868 7.21706 17.5923 7.72348 18.2122 7.72348H21.0374C21.6563 7.72348 22.1629 7.21706 22.1629 6.59731V3.90448C22.1629 3.28498 21.6563 2.77739 21.0374 2.77739H18.2122ZM22.1737 10.5723H19.974C20.1826 11.2536 20.2957 11.972 20.2957 12.7189C20.2957 16.8757 16.8152 20.2472 12.5235 20.2472C8.23292 20.2472 4.75233 16.8757 4.75233 12.7189C4.75233 11.972 4.8665 11.2536 5.07408 10.5723H2.77917V21.1333C2.77917 21.6802 3.22575 22.1251 3.77217 22.1251H21.1811C21.728 22.1251 22.1737 21.6802 22.1737 21.1333V10.5723ZM12.5236 7.58148C9.75192 7.58148 7.50358 9.75881 7.50358 12.4471C7.50358 15.1327 9.75192 17.3117 12.5236 17.3117C15.2968 17.3117 17.5452 15.1327 17.5452 12.4471C17.5452 9.75873 15.2968 7.58148 12.5236 7.58148Z"
            fill="black"
          />
        </svg>
        <span>@marketing_strategia</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      number: "",
      email: ""
    };
  },
  methods: {
    send() {
      // TODO запрос на сервер. доступ к полям через this.поле 
    }
  }
};
</script>

<style lang="scss">
.contacts {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
  background-repeat: no-repeat;
  background: url("../assets/4bg.jpg");
  background-size: 100% 100%;
  position: relative;

  .info {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 128px 0 0;
    min-width: 50%;

    span {
      text-transform: uppercase;
      font-size: 30px;
      line-height: 30px;
    }
  }

  .price {
    font-size: 30px;
    line-height: 38px;
    margin: 32px 0 128px;
  }

  .form {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    margin: 16px 0;

    input {
      width: 25%;
      border: 0;
      height: 40px;
      border-bottom: 5px solid #e52600 !important;
      border-top: 0px solid #e52600 !important;
      border-left: 0px solid #e52600 !important;
      border-right: 0px solid #e52600 !important;

      margin: 12px 0;
      background: rgba($color: #000, $alpha: 0);
      padding: 0 16px;
      position: relative;
      transition: 0.4s;

      &:focus {
        outline: 0;
        border: 5px solid #e52600 !important;
        margin: 9.5px 0;
      }

      &:active {
        border: 5px solid #e52600 !important;
        margin: 9.5px 0;
      }

      
    }
  }

  .contact-info {
    display: flex;
    justify-content: space-around;
    align-items: center;
    font-size: 24px;
    line-height: 30px;
    min-width: 30%;
    margin: 32px 0;

    .item {
      display: flex;
      justify-content: center;
      align-items: center;
      svg {
        width: 25px;
        height: 25px;
        margin: 8px;
      }
    }
  }
}
</style>
