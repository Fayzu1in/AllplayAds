<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <div class="wrapper">
      <div class="container">
        <div class="hero">
          <span
            ><img height="40px" src="./assets/logo_228_96.png" alt=""
          /></span>
          Лидирующий стриминговый сервис в Узбекистане
          <br />
          Мы предлагаем вам актуальную рекламу в нашем приложении.
        </div>
        <div class="orderTop">
          <div class="orderTop__header">Размещение рекламы</div>

          <div class="orderTop__links">
            <a
              class="orderTop__links-link"
              href="https://t.me/allplayallmovies"
            >
              <img src="./assets/telegram.png" alt="" /> @allplayallmovies
            </a>
            <a class="orderTop__links-link" href="tel:+998909113086"
              ><img src="./assets/phonecall.png" alt="" />+998 90 911 30 86</a
            >
          </div>
        </div>
        <div class="price">
          <!-- <div class="price__title">Прайс лист</div> -->
          <div class="price__cards">
            <div class="bkg">
              <div class="price__cards-card">
                <p class="currentPrice">20 сумов</p>
                <p class="currentPrice__subtitle">
                  За просмотр <br />
                  при покупке до 500 000 просмотров
                </p>
              </div>
            </div>
            <div class="bkg1">
              <div class="price__cards-card">
                <p class="currentPrice">15 сумов</p>
                <p class="currentPrice__subtitle">
                  За просмотр <br />
                  при покупке свыше 500 000 просмотров
                </p>
              </div>
            </div>
            <div class="bkg3">
              <div class="price__cards-card">
                <p class="currentPrice">12 сумов</p>
                <p class="currentPrice__subtitle">
                  За просмотр <br />
                  при покупке свыше 800 000 просмотров
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="requirements">
          <div class="requirements__header">Важно:</div>
          <ul class="requirements__list">
            <li>&#9632; Соотношение сторон должно быть 16x9</li>
            <li>
              &#9632; Реклама будет выходить только у бесплатных пользователей
              либо у пользователей с "Промо" подпиской
            </li>
            <li>
              &#9632; Перед публикацией, каждый рекламный ролик проходит
              модерацию в течении 24 часов
            </li>
            <li>
              &#9632; Длительность рекламного ролика не должна превышать 30
              секунд
            </li>
            <li>&#9632; Реклама имеется только в виде Pre-roll</li>
            <li>&#9632; При оплате через договор, НДС составляет 15%</li>
          </ul>
        </div>

        <div class="main">
          <p class="main__title">Платформы:</p>
          <div class="cards">
            <div class="platformTv">
              <div class="card">SMART TV</div>
            </div>
            <div class="platformPhone">
              <div class="card">Android и iOS</div>
            </div>
            <div class="platformWeb">
              <div class="card">Веб-сайт</div>
            </div>
          </div>
        </div>

        <div class="statistic">
          <img class="statistic__left" src="./assets/advertImg.webp" alt="" />
          <div class="statistic__right">
            <div class="statistic__right-header">Статистика</div>
            <p>10 000 - 15 000 просмотров в день!</p>
            <p>300 000 - 400 000 просмотров в месяц!</p>
            <p>
              <span class="statistic__right-header">Возрастная категория</span>
              <br />
              от 18 до 24: 33% <br />
              от 24 до 44: 52% <br />
              от 45 и старше: 15%
            </p>
          </div>
        </div>

        <div class="order">
          <div class="order__header">Заказать размещение рекламы</div>

          <a class="order__link" href="https://t.me/allplayallmovies">
            <img src="./assets/telegram.png" alt="" /> @allplayallmovies
          </a>
          <a class="order__link" href="tel:+998909113086"
            ><img src="./assets/phonecall.png" alt="" />+998 90 911 30 86</a
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: "App",
  components: {
    // HelloWorld
  },
};
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
}

body {
  background-color: #000;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
  color: #fff;
}
.container {
  width: 1268.92px;
  margin: 0 auto;
  @media screen and (max-width: 420px) {
    width: unset;
  }
}

.orderTop {
  padding-bottom: 30px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  @media screen and (max-width: 420px) {
    flex-direction: column;
    padding-bottom: unset;
  }
  &__header {
    font-size: 32px;
    @media screen and (max-width: 420px) {
      display: none;
    }
  }
  &__links {
    display: flex;
    justify-content: space-around;
    width: 400px;
    @media screen and (max-width: 420px) {
      display: none;
    }
    &-link {
      display: flex;
      align-items: center;
      color: #fff;
      text-decoration: none;
      transition: all 0.3s;
      &:hover {
        color: rgb(254, 153, 0);
      }
      img {
        height: 40px;
        padding-right: 5px;
      }
    }
  }
}

.main {
  line-height: 1.4rem;
  color: #999;

  padding-bottom: 30px;

  .cards {
    display: flex;
    justify-content: space-evenly;
    padding: 30px 0;
    @media screen and (max-width: 420px) {
      flex-direction: column;
      padding: 0 30px;
    }
    .platformTv {
      background-image: url(./assets/couch1.png);
      background-position: center;
      background-size: cover;
      @media screen and (max-width: 420px) {
        margin-bottom: 30px;
      }
    }
    .platformPhone {
      background-image: url(./assets/phone2.webp);
      background-position: center;
      background-size: cover;
      @media screen and (max-width: 420px) {
        margin-bottom: 30px;
      }
    }
    .platformWeb {
      background-image: url(./assets/laptop.jpg);
      background-position: center;
      background-size: cover;
    }
    .card {
      width: 350px;
      height: 200px;
      backdrop-filter: blur(2px);
      background-color: rgba(0, 0, 0, 0.494);
      background-color: rgba(0, 0, 0, 0.494);
      color: #fff;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 32px;
      text-align: center;
      @media screen and (max-width: 420px) {
        width: unset;
        font-size: 24px;
      }
    }
  }
  &__title {
    font-size: 32px;
    padding: 30px 0;
    color: #fff;
    @media screen and (max-width: 420px) {
      font-size: 24px;
      padding: 30px 30px;
    }
  }
}

.hero {
  display: flex;
  align-items: center;
  padding: 30px;
  justify-content: flex-start;
  margin-bottom: 30px;
  border-bottom: 2px solid rgb(254, 153, 0);
  @media screen and (max-width: 420px) {
    flex-direction: column;
    text-align: center;
    font-size: 16px;
  }
  span {
    padding-right: 15px;
    @media screen and (max-width: 420px) {
      padding-right: unset;
      height: 50px;
    }
  }
}
.price {
  color: #fff;
  line-height: 1.4rem;
  padding: 15px;
  margin: 30px 0;
  @media screen and (max-width: 420px) {
    margin: unset;
    padding: 0 30px;
  }

  &__title {
    font-size: 32px;
    padding: 30px 0;
  }

  &__cards {
    display: flex;
    justify-content: space-around;
    @media screen and (max-width: 420px) {
      flex-direction: column;
    }

    .bkg {
      background-image: url(./assets/image.png);
      background-position: center;
      background-size: cover;
      @media screen and (max-width: 420px) {
        margin-bottom: 30px;
      }
    }
    .bkg1 {
      background-image: url(./assets/image1.png);
      background-position: center;
      background-size: cover;
      @media screen and (max-width: 420px) {
        margin-bottom: 30px;
      }
    }
    .bkg3 {
      background-image: url(./assets/image2.png);
      background-position: center;
      background-size: cover;
      @media screen and (max-width: 420px) {
        margin-bottom: 30px;
      }
    }

    &-card {
      padding: 45px 15px;
      width: 300px;
      text-align: center;
      backdrop-filter: blur(2px);
      background-color: rgba(0, 0, 0, 0.494);
      @media screen and (max-width: 420px) {
        width: unset;
      }

      .currentPrice {
        font-size: 42px;
        color: #fff;
        padding-bottom: 30px;
        @media screen and (max-width: 420px) {
          font-size: 32px;
          padding-bottom: 20px;
        }

        &__subtitle {
          color: #999;
        }
      }
    }
  }
}
.requirements {
  color: #999;
  @media screen and (max-width: 420px) {
    padding: 0 30px;
  }
  &__header {
    font-size: 24px;
  }
  padding-bottom: 30px;
  li {
    list-style-type: none;
    line-height: 22px;
  }
}
.statistic {
  display: flex;

  justify-content: space-around;
  align-items: center;
  padding-bottom: 30px;
  border-bottom: 2px solid rgb(254, 153, 0);
  @media screen and (max-width: 420px) {
    flex-direction: column;
  }

  &__left {
    height: 360px;
    @media screen and (max-width: 420px) {
      display: none;
    }
  }
  &__right {
    padding: 30px;
    font-size: 18px;
    color: #999;
    @media screen and (max-width: 420px) {
      font-size: 16px;
      padding: unset;
    }
    &-header {
      color: rgb(254, 153, 0);
    }
  }
}
.order {
  display: flex;
  align-items: center;
  padding: 30px 0;

  @media screen and (max-width: 420px) {
    flex-direction: column;
    align-items: flex-start;
    padding: 10px 30px;
  }
  &__header {
    font-size: 18px;
    @media screen and (max-width: 420px) {
      font-size: 16px;
      padding-bottom: 10px;
    }
  }
  &__link {
    display: flex;

    align-items: center;
    padding-left: 20px;
    text-decoration: none;
    color: #fff;
    transition: all 0.3s;
    @media screen and (max-width: 420px) {
      padding: unset;
      padding-bottom: 10px;
      font-size: 16px;
    }
    &:hover {
      color: rgb(254, 153, 0);
    }
    img {
      height: 40px;
      @media screen and (max-width: 420px) {
        height: 24px;
      }
    }
  }
}
</style>
