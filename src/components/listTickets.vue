<template>
  <div class="list_tickets">
    <ticket v-for="item in 5" :key="item"/>
  </div>
</template>

<script>
import ticket from './ticket.vue'
export default {
  components: { ticket },

}
</script>

<style lang="scss">
.list_tickets {
  display: flex;
  flex-direction: column;
  width: 100%;
}
</style>