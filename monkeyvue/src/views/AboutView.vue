<template>
  <Cart
    v-for="monkey in store.cart"
    :key="monkey"
    :name="monkey.name"
    :cost="monkey.cost"
    :img="monkey.img"
  ></Cart>

  <div class="total">Total Cost: {{ total() }}</div>
</template>

<script>
import Cart from "../components/cart.vue";
import { store } from "../components/store";
export default {
  name: "CartView",
  components: {
    Cart,
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
        total += store.cart[i].cost * store.cart[i].count;
      }
      return total;
    },
  },
};
</script>

<style lang="scss" scoped></style>
