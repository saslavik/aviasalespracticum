<template>
  <div class="ticket">
    <div class="ticket_actions">
      <div class="ticket_bag"></div>
      <button class="ticket_button">Купить <br>за 4 675 Р</button>
      <div class="ticket_company">на Clickavia</div>
    </div>
    <div class="ticket_info">
      <div class="air_company">RUSSIA</div>
      <div class="air_line dotted">
        <div class="ticket_departure">
          <div class="departure_time d_time">00:05</div>
          <div class="departure_city">Москва</div>
          <div class="departure_date">24 фев 2018, Сб</div>
        </div>
        <div class="ticket_time">
          <div class="air_time">Всего: 5ч</div>
          <div class="ticket_time_line">
            <div class="circle"></div>
            <div class="circle_line"></div>
            <div class="circle"></div>
          </div>
          <div class="ticket_shortCity">
            <span>VKO</span>
            BCN
          </div>
        </div>
        <div class="ticket_destination">
          <div class="destination_time d_time">03:05</div>
          <div class="destination_city">Барселона</div>
          <div class="destination_date">24 фев 2018, Сб</div>
        </div>
      </div>
      <div class="air_line">
        <div class="ticket_departure">
          <div class="departure_time d_time">00:05</div>
          <div class="departure_city">Москва</div>
          <div class="departure_date">24 фев 2018, Сб</div>
        </div>
        <div class="ticket_time">
          <div class="air_time">Всего: 5ч</div>
          <div class="ticket_time_line">
            <div class="circle"></div>
            <div class="circle_line"></div>
            <div class="circle"></div>
          </div>
          <div class="ticket_shortCity">
            <span>VKO</span>
            BCN
          </div>
        </div>
        <div class="ticket_destination">
          <div class="destination_time d_time">03:05</div>
          <div class="destination_city">Барселона</div>
          <div class="destination_date">24 фев 2018, Сб</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  .ticket {
    display: flex;
    background-color: #fff;
    margin-bottom: 20px;
    margin-left: 16px;
    &_company {
      color: #A0B0B9;
      font-size: 12px;
      text-align: center;
    }
    &_actions{
      border-right: 1px solid #EAEAEA;
    }
  }
  .ticket_button {
    width: 160px;
    margin: 22px 22px 6px 22px;
    padding: 6px;
  }
  .ticket_info {
    display: flex;
    flex-direction: column;
    flex-grow: 5;
    padding: 16px;
    font-size: 12px;
    color: #9CA5A8;
    white-space: nowrap;
  }
  .air_line {
    display: flex;
    padding: 15px 0;
  }
  .air_time {
    display: flex;
    justify-content: center;
  }
  .dotted {
      border-bottom: 1px dashed #DDDDDD;
    }
  .ticket_time{
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: 100%;
    flex-grow: 5;
    padding: 0 15px;
    &_line {
      display: flex;
      justify-content: space-between;
    }
  }
  .ticket_shortCity {
    display: flex;
    // flex-direction: column;
    justify-content: space-between;
    font-size: 10px;
    color: #4A4A4A;
    font-weight: bold;
  }
  .d_time {
    color: #323333;
    font-size: 28px;
  }
  .circle {
    width: 11px;
    height: 11px;
    border: 1px solid #A0B0B9;
    border-radius: 50%;
    &_line {
      border-top: 1px solid #A0B0B9;
      flex-grow: 999;
      height: 1px;
      margin: auto 0;
    }
  }
</style>