<template>
  <div class="home">
    <div class="main">
      <div class="logo">
          <div class="logoImg">
            <img src="../assets/svg/aviasales.svg" alt="">
          </div>
          <p>aviasales</p>
      </div>
      <div class="container">
        <div class="main__finder">
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
              <button @click.prevent="">Найти билеты</button>
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
  height: 100vh;
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
  height: 80vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
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
    button {
      padding: 15px 50px;
      background-color: #FF9241;
      color: white;
      font-size: 28px;
      border-radius: 4px;
      border: none;
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
  }
}
</style>
