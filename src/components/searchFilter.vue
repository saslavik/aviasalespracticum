<template>
  <div class="searchFilter">
    <div class="filter">
      <div class="item">
        <div class="item_title">Пересадки</div>
        <div class="item_container">
          <div class="item_transplants">
            <div class="checklabel">
              <input type="checkbox" name="transplants" value="all"> Все
            </div>

          </div>
          <div class="item_transplants">
            <div class="checklabel">
              <input type="checkbox" name="transplants" value="without"> Без пересадок
            </div>
            7 712 ₽
          </div>
          <div class="item_transplants">
            <div class="checklabel">
              <input type="checkbox" name="transplants" value="1">1 пересадка
            </div>
            11 150 ₽
          </div>
          <div class="item_transplants">
            <div class="checklabel">
              <input type="checkbox" name="transplants" value="2">2 пересадки
            </div>
            16 821 ₽
          </div>
          <div class="item_transplants">
            <div class="checklabel">
              <input type="checkbox" name="transplants" value="3">3 пересадки <br>
            </div>
            23 986 ₽
          </div>
        </div>
      </div>
      <div class="item">
        <div class="item_title">Время вылета и прибытия</div>
        <div class="item_container">
          <div class="item_startTime">
            <div class="city_destinations"></div>
            <div class="city_time"></div>
          </div>
        </div>
      </div>
      <div class="item">
        <div class="item_title">Багаж</div>
        <div class="item_container">
          <div class="item_startTime">
            <div class="city_destinations"></div>
            <div class="city_time"></div>
          </div>
        </div>
      </div>
      <div class="item">
        <div class="item_title">Длительность пересадки</div>
        <div class="item_container">
          <div class="item_startTime">
            <div class="city_destinations"></div>
            <div class="city_time"></div>
          </div>
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
  .filter {
    background-color: #fff;
    width: 300px;
    border-radius: 4px;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    .item {
      margin: 15px;
    }
    .item_container {
      display: flex;
      flex-direction: column;
    }
    .item_transplants {
      display: flex;
      justify-content: space-between;
    }
    .checklabel {
      display: flex;
      // justify-content: start;
      // vertical-align: center;
      // text-align: left;
      white-space: nowrap;
      input {
        width: 13px;
        margin: auto 5px auto 0;
      }
    }
  }
</style>