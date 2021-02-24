<template>
  <div class="home">
    <div class="main main_full">
      <div class="logo">
          <div class="logoImg">
            <img src="../assets/svg/aviasales.svg" alt="">
          </div>
          <p>aviasales</p>
      </div>
      <div class="container">
        <div class="main__finder main__finder_full">
          <h2>Поиск дешевых авиабилетов</h2>
          <h6>Лучший способ купить авиабилетов дешево</h6>
          <form class="main__form">
            <div class="main__form_inputs">
              <input type="select" class="departure">
              <input type="select" class="destination">
              <input type="date" class="date">
              <input type="date" class="date">
              <input type="number" class="passangers">
            </div>
            <div class="submit">
              <button @click.prevent="" class="btn_airplane">Найти билеты</button>
            </div>
          </form>
        </div>
      </div>
    </div>
    <top-destinations/>
    <best-price/>
    <special-price/>
    <img alt="Vue logo" src="../assets/logo.png">
  </div>
</template>

<script>
import BestPrice from '../components/bestPrice.vue'
import SpecialPrice from '../components/specialPrice.vue'
import topDestinations from '../components/topDestinations.vue'
// @ is an alias to /src

export default {
  components: { topDestinations, BestPrice, SpecialPrice },
  name: 'Home',

}
</script>

<style lang="scss">

.main {
  background: linear-gradient(135.21deg, #00B0DE 0.36%, #01AEDC 4.04%, #02ABDB 7.77%, #02ABDB 11.48%, #02ABDB 11.7%, #196EBD 100%);
  width: 100wh;
  &_full{
    height: 100vh;
  }
  &__form {
    display: flex;
  }
  .submit {
    margin: 40px 0;
  }
}

.logo {
  display: inline-flex;
  color: #fff;
  justify-content: center;
  text-align: center;
  line-height: 30px;
  margin: 10px;
  img {
    margin-right: 10px;
  }
  @media screen and (min-width: 769px) {
    margin: 12px 100px;
  }
  p {
    @media screen and (max-width: 480px) {
      display: none;
    }
  }
}

.main__finder {
  margin: 0 0px;
  color: white;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  &_full {
  height: 80vh;
  }
  h2 {
    font-size: 40px;
    font-weight: bold;
    @media screen and(max-width: 768px) {
      font-size: 32px;
    }
    @media screen and(max-width: 480px) {
      font-size: 20px;
    }
  }
  h6 {
    font-size: 24px;
    font-weight: bold;
    @media screen and(max-width: 768px) {
      font-size: 20px;
    }
    @media screen and(max-width: 480px) {
      display: none;
    }
  }
  .main__form {
    display: flex;
    flex-direction: column;

    &_inputs {
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      margin: 40px 0;
      @media screen and(max-width: 768px) {
        margin: 32px 0;
      }
      @media screen and(max-width: 480px) {
        margin: 16px 0;
      }
      input {
        flex-grow: 1;
        margin-right: 2px;
        width: 19%;
        &:first-child {
          border-radius: 4px 0 0 4px;
        }
        &:last-child {
          border-radius: 0 4px 4px 0;
        }
        @media screen and (max-width: 768px) {
          width: 49%;
          flex-grow: 1;
          margin-bottom: 2px;
          &.date {
            width: 24%;
            flex-grow: 1;
          }
          &:first-child {
            border-radius: 4px 0 0 0;
          }
          &:nth-child(2) {
            border-radius: 0 4px 0 0;
          }
          &:nth-child(3) {
            border-radius: 0 0 0 4px;
          }
          &:last-child {
            border-radius: 0 0 4px 0;
        }
        }
        @media screen and(max-width: 480px) {
        width: 100%;
        border-radius: 0 !important;
        &:first-child{
          border-radius: 4px 4px 0 0 !important;
        }
        &:last-child{
          border-radius: 0 0 4px 4px !important;
        }
        }
      }
    }
    
    .btn_airplane {
      padding: 15px 50px;
      font-size: 28px;
      position: relative;
      &:after {
        content: '';
        position: absolute;
        mask-image: url(../assets/svg/aero.svg);
        width: 26px;
        height: 21px;
        background-color: #fff;
        mask-size: cover;
        -webkit-mask-size: cover;
        margin-left: 10px;

      }
    }
    &_search{
      flex-direction: row;
      button {
        padding: 0 15px;
        font-weight: bold;
        font-size: 20px;
        height: 100%;
        margin-left: 5px;
        white-space: nowrap;
        text-align: center;
      }
      }
  }
}
</style>
