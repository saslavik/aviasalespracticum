<template>
  <div class="wrapper-content">
    <div class="topDestinations">
      <div class="container">

        <div class="elementLogo">
          <img src="../assets/svg/Group.svg" alt="">
        </div>

        <div class="elementTitle">
          Популярные направления перелетов<br>из города Москва
        </div>

        <div class="chooseDestinations">
          <div class="anywhere svg">Куда угодно</div>
          <div class="sun svg">Солнце и море</div>
          <div class="shopping svg">Шоппинг, город</div>
          <div class="history svg">Культура и история</div>
          <div class="club svg">Ночная жизнь</div>
          <div class="kids svg">Отдых с детьми</div>
        </div>
        <div class="cardList">
          <div class="card">
            <div class="cardImg"><img src="../assets/img/krasnodar.jpg" alt=""></div>
            <div class="cardDescr">
              <div class="cardCountry">
                <div class="flag"><img src="../assets/img/flagru.jpg" alt=""></div>
                <div class="city">
                  Краснодар
                  <p>Россия</p>
                </div>
              </div>
              <div class="cardPrice">
                Найти от 1 212 Р
                <p>12 марта</p>
              </div>
            </div>
          </div>
          <div class="card">
            <div class="cardImg"><img src="../assets/img/krasnodar.jpg" alt=""></div>
            <div class="cardDescr">
              <div class="cardCountry">
                <div class="flag"><img src="../assets/img/flagru.jpg" alt=""></div>
                <div class="city">
                  Краснодар
                  <p>Россия</p>
                </div>
              </div>
              <div class="cardPrice">
                Найти от 1 212 Р
                <p>12 марта</p>
              </div>
            </div>
          </div>
          <div class="card">
            <div class="cardImg"><img src="../assets/img/krasnodar.jpg" alt=""></div>
            <div class="cardDescr">
              <div class="cardCountry">
                <div class="flag"><img src="../assets/img/flagru.jpg" alt=""></div>
                <div class="city">
                  Краснодар
                  <p>Россия</p>
                </div>
              </div>
              <div class="cardPrice">
                Найти от 1 212 Р
                <p>12 марта</p>
              </div>
            </div>
          </div>
          <div class="card">
            <div class="cardImg"><img src="../assets/img/krasnodar.jpg" alt=""></div>
            <div class="cardDescr">
              <div class="cardCountry">
                <div class="flag"><img src="../assets/img/flagru.jpg" alt=""></div>
                <div class="city">
                  Краснодар
                  <p>Россия</p>
                </div>
              </div>
              <div class="cardPrice">
                Найти от 1 212 Р
                <p>12 марта</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
  .topDestinations {
    margin: 30px 0;
    background-color: #ececec;
    color: #4A4A4A;
  }
  .elementLogo {
    display: flex;
    justify-content: center;
    width: 64px;
    height: 64px;
    margin: 20px auto;
  }

  .elementTitle {
    display: flex;
    justify-content: center;
    text-align: center;
    font-size: 24px;
    line-height: 36px;
    @media screen and(max-width: 480px) {
      font-size: 18px;
    }
  }

.chooseDestinations{
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  .svg {
    display: flex;
    flex-direction: column;
    text-align: center;
    max-width: 90px;
    margin-top: 120px;
    margin-right: 16px;
    flex: 12px;
    line-height: 20px;
    position: relative;
    &::before {
      content: '';
      justify-content: center;
      text-align: center;
      width: 48px;
      height: 48px;
      border-radius: 50%;
      position: absolute;
      top: -58px;
      left: 21px;
      mask-position: center;
      mask-size: 50%;
      -webkit-mask-size: 50%;
      mask-repeat: no-repeat;
      background-color: #A0B0B9;
    }
  }
  .anywhere {
    &::before {
      content: '';
      -webkit-mask-image: url(../assets/svg/svg-5.svg);
      mask-image: url(../assets/svg/svg.svg);

    }
  }
  .sun{
    &::before {
      content: '';
      -webkit-mask-image: url(../assets/svg/svg-4.svg);
      mask-image: url(../assets/svg/svg.svg);

    }
  }
  .shopping{
    &::before {
      content: '';
      -webkit-mask-image: url(../assets/svg/svg-3.svg);
      mask-image: url(../assets/svg/svg.svg);

    }
  }
  .history{
    &::before {
      content: '';
      -webkit-mask-image: url(../assets/svg/svg-2.svg);
      mask-image: url(../assets/svg/svg.svg);

    }
  }
  .club{
    &::before {
      content: '';
      -webkit-mask-image: url(../assets/svg/svg-1.svg);
      mask-image: url(../assets/svg/svg.svg);

    }
  }
  .kids{
    &::before {
      content: '';
      -webkit-mask-image: url(../assets/svg/svg.svg);
      mask-image: url(../assets/svg/svg.svg);

    }
  }

}
.cardList {
  margin: 40px 0;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  background-color: #ececec;
  @media screen and(max-width: 768px) {
    flex-direction: column;
  }
  .card {
    width: 49%;
    margin: 10px 0;
    box-shadow: 0px 2px 12px rgba(0, 75, 93, 0.12);
    border-radius: 8px;
    overflow: hidden;
    background-color: #fff;
    @media screen and(max-width: 768px) {
      width: 100%;
    }
    img {
      width: 100%;
    }
  }
  .cardDescr {
    display: flex;
    justify-content: space-between;
    margin: 24px;
    font-size: 22px;
    @media screen and(max-width: 480px) {
      font-size: 16px;
    }
    .cardCountry {
      display: flex;

      .flag {
        margin-right: 16px;
        @media screen and(max-width: 480px) {
          display: none;
        }
      }
      .city {
        color: #5B5B5C;
      }
    }
    .cardPrice {
      color: #00BAE8;
      justify-content: end;
      text-align: right;
    }
    p {
      font-size: 12px;
      color: #A0B0B9;
    }
  }

}
</style>