<template>
  <div class="card">
    <h2>{{ name }}</h2>
    <img :src="img" :alt="Monkey" />
    <p>Price: {{ cost }}</p>
    <button @click="remove">Remove</button>
  </div>
</template>

<script>
import { store } from "../components/store";

export default {
  name: "Cart",
  props: {
    name: String,
    img: String,
    cost: Number,
  },
  methods: {
    remove() {
      store.cart.splice(this.index, 1);
    },
  },
};
</script>

<style>
.card {
  height: fit-content;
  display: flex;
  flex-direction: column;
  padding: 1rem 1rem 2rem;
  background: #f8f3e8;
  box-shadow: 0 0 40px rgba(0, 0, 0, 0.2), 0 0 40px rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  margin-bottom: 30px;
}
.card > img {
  width: 100%;
  height: auto;
}
</style>
