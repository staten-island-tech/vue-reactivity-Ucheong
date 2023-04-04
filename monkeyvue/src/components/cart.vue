<template>
  <div class="cart">
    <h2>{{ name }}</h2>
    <img :src="img" :alt="name" />
    <p>Price: ${{ cost }}</p>
    <button @click="remove(name)">Remove</button>
  </div>
</template>

<script>
import { store } from "../components/store";

export default {
  name: "cart",
  props: {
    name: String,
    img: String,
    cost: Number,
  },
  methods: {
    remove(name) {
      let monkey = store.cart.find((monkey) => monkey.name === name);
      store.cart.splice(monkey, 1);
    },
  },
};
</script>

<style>
.cart {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;
  background: #f8f3e8;
  border-radius: 3px;
  margin-bottom: 30px;
  width: 20vw;
}
.cart > img {
  width: 100%;
  height: auto;
}
</style>
