<template>
  <div class="search">
    <div class="main">
      <div class="logo">
          <div class="logoImg">
            <img src="../assets/svg/aviasales.svg" alt="">
          </div>
          <p>aviasales</p>
      </div>
      <div class="container">
        <div class="main__finder">
          <form class="main__form main__form_search">
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
    <div class="container">
      <div class="search_container">
        <search-filter/>
        <list-tickets/>
      </div>
    </div>
  </div>
</template>

<script>
import ListTickets from '../components/listTickets.vue'
import searchFilter from '../components/searchFilter.vue'
export default {
  components: { searchFilter, ListTickets },

}
</script>

<style lang="scss">
  .search {
    background-color: #EAEAEA;
    .search_container {
      display: flex;
      margin-top: 40px;
    }
  }
</style>