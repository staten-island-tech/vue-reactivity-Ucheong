<template>
  <h1>Welcome to the Monkey Shop!</h1>
  <h2>(Note that you can not own more than one of each of these monkeys)</h2>
  <div class="home">
    <Card
      v-for="monkey in monkeys"
      :key="monkey"
      :name="monkey.name"
      :description="monkey.description"
      :cost="monkey.cost"
      :stock="monkey.stock"
      :img="monkey.img"
    />
  </div>
</template>

<script>
import Card from "../components/card.vue";

export default {
  components: {
    Card,
  },
  data() {
    return {
      monkeys: [
        {
          name: "Monkey1",
          description: "Who are you?",
          cost: "15k",
          stock: 20,
          img: "Monkey1.jpg",
        },
        {
          name: "Monkey2",
          description: "You",
          cost: "20k",
          stock: 15,
          img: "Monkey2.jpg",
        },
        {
          name: "Monkey3",
          description: "Bodyguard",
          cost: "30k",
          stock: 5,
          img: "Monkey3.jpg",
        },
        {
          name: "Monkey4",
          description: "I like bananas",
          cost: "10k",
          stock: 30,
          img: "Monkey4.jpg",
        },
        {
          name: "Monkey5",
          description: "Most basic monkey monkey out there",
          cost: "25k",
          stock: 10,
          img: "Monkey5.jpg",
        },
        {
          name: "Monkey6",
          description: "Curious George",
          cost: "15k",
          stock: 18,
          img: "Monkey6.jpg",
        },
        {
          name: "Monkey7",
          description: "Your fav hitman",
          cost: "40k",
          stock: 3,
          img: "Monkey7.jpg",
        },
        {
          name: "Monkey8",
          description: "😩",
          cost: "22k",
          stock: 9,
          img: "Monkey8.jpg",
        },
        {
          name: "Monkey9",
          description: "Snorlax",
          cost: "33k",
          stock: 2,
          img: "Monkey9.jpg",
        },
        {
          name: "Monkey10",
          description: "I love me some Pepsi",
          cost: "11k",
          stock: 23,
          img: "Monkey10.jpg",
        },
        {
          name: "Monkey11",
          description: "I'm your clown",
          cost: "29k",
          stock: 7,
          img: "Monkey11.jpg",
        },
        {
          name: "Monkey12",
          description: "I'm a zesty mf",
          cost: "30k",
          stock: 7,
          img: "Monkey12.jpg",
        },
        {
          name: "Monkey13",
          description: "🗿",
          cost: "24k",
          stock: 8,
          img: "Monkey13.jpg",
        },
        {
          name: "Monkey14",
          description: "I'm about to pass, these cigs don't taste good no more",
          cost: "8k",
          stock: 63,
          img: "Monkey14.jpg",
        },
        {
          name: "Monkey15",
          description: "Your Diaper Monkey",
          cost: "13k",
          stock: 16,
          img: "Monkey15.jpg",
        },
        {
          name: "Monkey16",
          description: "THe one and only sniper monkey",
          cost: "62k",
          stock: 1,
          img: "Monkey16.jpg",
        },
        {
          name: "Monkey17",
          description: "I don't play no games",
          cost: "53k",
          stock: 2,
          img: "Monkey17.jpg",
        },
        {
          name: "Monkey18",
          description: "I got a legendary pump shotgun",
          cost: "60k",
          stock: 2,
          img: "Monkey18.jpg",
        },
        {
          name: "Monkey19",
          description: "What gun do I have?",
          cost: "57k",
          stock: 3,
          img: "Monkey19.jpg",
        },
        {
          name: "Monkey20",
          description: "I will raid you; Professionally trained by cartels",
          cost: "100k",
          stock: 100000,
          img: "Monkey20.jpg",
        },
        {
          name: "Monkey21",
          description: "🚬",
          cost: "50k",
          stock: 20,
          img: "Monkey21.jpg",
        },
        {
          name: "Monkey22",
          description: "Faded than a hoe",
          cost: "100k (included)",
          stock: 100,
          img: "Monkey22.jpg",
        },
        {
          name: "Monkey23",
          description: "Prisoner Monkey",
          cost: "1",
          stock: 2000000,
          img: "Monkey23.jpg",
        },
        {
          name: "Monkey24",
          description: "Faded than a hoe",
          cost: "40k",
          stock: 300,
          img: "Monkey24.jpg",
        },
        {
          name: "Monkey25",
          description: "I will beat anyone up for u",
          cost: "200k",
          stock: 1000,
          img: "Monkey25.jpg",
        },
        {
          name: "Monkey26",
          description: "I'm a thief",
          cost: "1k",
          stock: 1,
          img: "Monkey26.jpg",
        },
        {
          name: "Monkey27",
          description: "Leader of the Camorra",
          cost: "1million",
          stock: 1,
          img: "Monkey27.jpg",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
