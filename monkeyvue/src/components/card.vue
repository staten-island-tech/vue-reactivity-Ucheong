<template>
  <div class="card">
    <h2>{{ name }}</h2>
    <img :src="img" :alt="Monkey" />
    <p>Description: {{ description }}</p>
    <p>Price: ${{ cost }}</p>
    <button @click="add">Add to Cart</button>
  </div>
</template>

<script>
import { reactive } from 'vue';
export default {
  name: "card",
  props: {
    name: String,
    description: String,
    img: String,
    cost: Number,
  },
  methods: {
    add() {
      cart.push({
        name: this.name,
        img: this.img,
        cost: this.cost,
      });
    },
  },
};
export const cart = reactive([])
</script>

<style>
.card {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;
  background: #f8f3e8;
  border-radius: 3px;
  margin-bottom: 30px;
  width: 20vw;
}
.card > img {
  height: 60%;
  width: 60%;
}
</style>
