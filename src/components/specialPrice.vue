<template>
  <div class="specialPrice">
    <div class="spContainer">
      <div class="spTitle">Спецпредложение на авиабилеты</div>
      <div class="spCardList">
        <div class="spCard">
          <div class="spCardTitle">Билеты от 499 рублей!</div>
          <div class="spCardDescr">
            <div class="spCompany">
              <img src="../assets/img/pobeda.jpg" alt="">
              <div class="spPrice">
                от <span>499 P</span>
                <p>Осталось 45 дней</p>
              </div>
            </div>
            <div class="spDescr">
              Билеты от 499 рублей! Специальное предложение от авиакомпании Победа
            </div>
            <div class="spBtn">Узнать подробности</div>
          </div>
        </div>
        <div class="spCard">
          <div class="spCardTitle">В Лос-Анджелес от 22...</div>
          <div class="spCardDescr">
            <div class="spCompany">
              <img src="../assets/img/pobeda.jpg" alt="">
              <div class="spPrice">
                от <span>499 P</span>
                <p>Осталось 45 дней</p>
              </div>
            </div>
            <div class="spDescr">
              Из Москвы в США от 22360 рублей! Специальное предложение от авиакомпании Lufthansa
            </div>
            <div class="spBtn">Узнать подробности</div>
          </div>
        </div>
        <div class="spCard">
          <div class="spCardTitle">В Нью-Йорк от 20 6…</div>
          <div class="spCardDescr">
            <div class="spCompany">
              <img src="../assets/img/pobeda.jpg" alt="">
              <div class="spPrice">
                от <span>499 P</span>
                <p>Осталось 45 дней</p>
              </div>
            </div>
            <div class="spDescr">
              Из Москвы в США от 22360 рублей! Специальное предложение от авиакомпании Lufthansa
            </div>
            <div class="spBtn">Узнать подробности</div>
          </div>
        </div>
      </div>
      <div class="spSeeAll">
        <a href="">Смотреть все спецпредложения</a>
        * средняя цена по направлению
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.specialPrice {
  background: linear-gradient(135.21deg, #00B0DE 0.36%, #01AEDC 4.04%, #02ABDB 7.77%, #02ABDB 11.48%, #02ABDB 11.7%, #196EBD 100%);
  color: #fff;
  padding: 24px 0;
  .spContainer {
    max-width: 1040px;
    margin: auto;
    @media screen and(max-width: 768px) {
      padding: 15px;
    }
  }
  .spTitle {
    font-size: 30px;
    font-weight: 500;
  }
  .spCardList {
    margin: 20px 0;
    display: flex;
    justify-content: space-between;
    @media screen and(max-width: 480px) {
      flex-direction: column;
    }
    .spCard {
      width: 30%;
      display: flex;
      flex-direction: column;
      background-color: #fff;
      @media screen and(max-width: 768px) {
        width: 33%;
      }
      @media screen and(max-width: 480px) {
        width: 100%;
        margin-bottom: 10px;
      }
      &Title{
        background-color: #CD2027;
        padding: 22px 16px;
        font-size: 16px;
      }
      &Descr{
        padding: 16px;
        height: 100%;
        color: #242424;
        display: flex;
        flex-direction: column;
        justify-content:space-between;
        .spCompany {
          display: flex;
          justify-content: space-between;
          text-align: right;
          font-size: 12px;
          @media screen and(max-width: 768px) {
            img{
              max-width: 50px;
            }
          }
          span {
            font-size: 16px;
          }
          p{
            color: #D93633;
          }
        }
        .spDescr {
          margin: 12px 0;
          font-size: 12px;
        }
        .spBtn {
          margin-top: 40px;
          text-align: center;
          color: #CD1F27;
          border: 2px solid #CD1F27;
          border-radius: 3px;
          padding: 10px 0;
        }
      }
    }
  }
  .spSeeAll {
    display: flex;
    justify-content: space-between;
    font-size: 16px;
  }
}
</style>