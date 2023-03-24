<template>
  <div class="card">
    <h2>{{ title }}</h2>
    <img :src="img" alt="" />
    <p>{{ description }}</p>
    <p>{{ cost }}</p>
    <p>{{ stock }}</p>
    <button>Add to Cart</button>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    title: String,
    description: String,
    img: String,
    cost: Number,
    stock: Number,
  },
};
</script>

<style lang="scss" scoped></style>
