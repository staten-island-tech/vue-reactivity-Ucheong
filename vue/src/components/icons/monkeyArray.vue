<template>
  <div v-for="monkey in monkeys" :key="monkey">{{ monkey }}</div>
</template>

<script>
export default {
  name: "Monkeys",
  components: {},
  data() {
    return {
      monkeys: ["../imgs.Monkey1.jpg", ""],
    };
  },
};
</script>

<style></style>
