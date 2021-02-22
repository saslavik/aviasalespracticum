<template>
<div class="wrapper-content">
  <div class="container">
    <div class="bestPrice">
      <div class="elementLogo">
        <img src="../assets/svg/sectionBestPrice.svg" alt="">
      </div>
      <div class="elementTitle">
        Лучшие цены на авиабилеты за последний месяц
      </div>
      <div class="bestPriceList">
        <div class="bpCity">
          <div class="cityTitle">
            <div class="bpFlag"><img src="../assets/img/flagru.jpg" alt=""></div>
            <div class="bpTitle">
              Симферополь (Крым)
              <p>Крым</p>
            </div>
          </div>
          <ul class="list">
            <li>Из Москвы <span>от 4 813 Р</span></li>
            <li>Из Санкт-Петербурга <span>от 14 813 Р</span></li>
            <li>Из Новосибирска <span>от 15 813 Р</span></li>
            <li>Из Екатеринбурга <span>от 24 813 Р</span></li>
            <li>Из Челябинска <span>от 7 813 Р</span></li>
          </ul>
        </div>
        <div class="bpCity">
          <div class="cityTitle">
            <div class="bpFlag"><img src="../assets/img/flagru.jpg" alt=""></div>
            <div class="bpTitle">
              Кишинёв
              <p>МОЛДАВИЯ</p>
            </div>
          </div>
          <ul class="list">
            <li>Из Москвы <span>от 4 813 Р</span></li>
            <li>Из Санкт-Петербурга <span>от 14 813 Р</span></li>
            <li>Из Новосибирска <span>от 15 813 Р</span></li>
            <li>Из Екатеринбурга <span>от 24 813 Р</span></li>
            <li>Из Челябинска <span>от 7 813 Р</span></li>
          </ul>
        </div>
        <div class="bpCity">
          <div class="cityTitle">
            <div class="bpFlag"><img src="../assets/img/flagru.jpg" alt=""></div>
            <div class="bpTitle">
              Ереван
              <p>АРМЕНИЯ</p>
            </div>
          </div>
          <ul class="list">
            <li>Из Москвы <span>от 4 813 Р</span></li>
            <li>Из Санкт-Петербурга <span>от 14 813 Р</span></li>
            <li>Из Новосибирска <span>от 15 813 Р</span></li>
            <li>Из Екатеринбурга <span>от 24 813 Р</span></li>
            <li>Из Челябинска <span>от 7 813 Р</span></li>
          </ul>
        </div>
      </div>
      <div class="bpNote">
        Мы знаем, где купить авиабилеты дешево. Билеты на самолет в 220 стран мира.<br>Поиск и сравнение цен на авиабилеты среди 100 агентств и 728 авиакомпаний.
        <p>Цены, найденные пользователями за последние 48 часов, не являются офертой.</p>
      </div>
    </div>
  </div>
</div>
</template>

<style lang="scss">
.bestPrice {
  color: #5B5B5C;
}
.bestPriceList{
  display: flex;
  justify-content: space-between;
  @media screen and(max-width: 768px) {
    flex-direction: column;
  }
  .bpCity {
    width: 27%;
    @media screen and(max-width: 768px) {
      width: 100%;
    }
    .cityTitle {
      display: flex;
      font-size: 22px;
      margin: 20px 0;
      .bpFlag {
        margin-right: 12px;
      }
      p {
        font-size: 12px;
        color: #A0B0B9;
      }
    }
  }
  li {
    font-size: 16px;
    display: flex;
    justify-content: space-between;
    margin: 16px 0;
    span {
      color: #00BAE8;
    }
  }
}
.bpNote {
  display: flex;
  flex-direction: column;
  text-align: center;
  justify-content: center;
  font-size: 16px;
  color: #4A4A4A;
  line-height: 26px;
  margin: 80px 0;
  p {
    font-size: 14px;
    color: #A0B0B9;
    margin: 16px 0;
  }
}
</style>