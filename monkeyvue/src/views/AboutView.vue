<template>
  <div class="shoppingCart">
    <cart
      v-for="monkey in store.cart"
      :key="monkey"
      :name="monkey.name"
      :cost="monkey.cost"
      :img="monkey.img"
    ></cart>
  </div>

  <div class="total">Total Cost: ${{ total() }}</div>
</template>

<script>
import cart from "../components/cart.vue";
import { store } from "../components/store";
export default {
  components: {
    cart,
  },
  data() {
    return {
      store,
    };
  },
  methods: {
    total() {
      let total = 0;
      for (let i = 0; i < store.cart.length; i++) {
        total += store.cart[i].cost;
      }
      return total;
    },
  },
};
</script>

<style>
.shoppingCart {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-evenly;
}

.total {
  text-align: center;
}
</style>
