<template>
  <div class="card">
    <h2>{{ name }}</h2>
    <img :src="img" :alt="Monkey" />
    <p>Description: {{ description }}</p>
    <p>Price: {{ cost }}</p>
    <p>Stock: {{ stock }} left</p>
    <button @click="add">Add to Cart</button>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    name: String,
    description: String,
    img: String,
    cost: Number,
    stock: Number,
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
