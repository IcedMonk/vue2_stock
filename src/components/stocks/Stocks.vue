<template>
  <div>
    <app-stock v-for="stock in stocks" :stock="stock"></app-stock>
  </div>
</template>


<script>
import Stock from './Stock.vue';
export default {
  data() {
    return {
      stocks: [
        {id: 1, name: 'BMW', price: 5},
        {id: 2, name: 'Porche', price: 2},
        {id: 3, name: 'Lamborghini', price: 9}
      ]
    }
  },
  components: {
    appStock: Stock
  }
}
</script>
