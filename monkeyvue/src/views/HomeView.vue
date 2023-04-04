<template>
  <h1 class="welcome">Welcome to the Monkey Shop!</h1>
  <div class="home">
    <card
      v-for="monkey in monkeys"
      :key="monkey"
      :name="monkey.name"
      :description="monkey.description"
      :cost="monkey.cost"
      :img="monkey.img"
    >
    </card>
  </div>
</template>

<script>
import card from "../components/card.vue";
import { store } from "../components/store";

export default {
  components: {
    card,
  },
  data() {
    return {
      store,
      monkeys: [
        {
          name: "Monkey1",
          description: "Who are you?",
          cost: 15000,
          img: "Monkey1.jpg",
        },
        {
          name: "Monkey2",
          description: "You",
          cost: 20000,
          img: "Monkey2.jpg",
        },
        {
          name: "Monkey3",
          description: "Bodyguard",
          cost: 30000,
          img: "Monkey3.jpg",
        },
        {
          name: "Monkey4",
          description: "I like bananas",
          cost: 10000,
          img: "Monkey4.jpg",
        },
        {
          name: "Monkey5",
          description: "Most basic monkey monkey out there",
          cost: 25000,
          img: "Monkey5.jpg",
        },
        {
          name: "Monkey6",
          description: "Curious George",
          cost: 15000,
          img: "Monkey6.jpg",
        },
        {
          name: "Monkey7",
          description: "Your fav hitman",
          cost: 40000,
          img: "Monkey7.jpg",
        },
        {
          name: "Monkey8",
          description: "😩",
          cost: 22000,
          img: "Monkey8.jpg",
        },
        {
          name: "Monkey9",
          description: "Snorlax",
          cost: 33000,
          img: "Monkey9.jpg",
        },
        {
          name: "Monkey10",
          description: "I love me some Pepsi",
          cost: 11000,
          img: "Monkey10.jpg",
        },
        {
          name: "Monkey11",
          description: "I'm your clown",
          cost: 29000,
          img: "Monkey11.jpg",
        },
        {
          name: "Monkey12",
          description: "I'm a zesty mf",
          cost: 30000,
          img: "Monkey12.jpg",
        },
        {
          name: "Monkey13",
          description: "🗿",
          cost: 24000,
          img: "Monkey13.jpg",
        },
        {
          name: "Monkey14",
          description: "I'm about to pass, these cigs don't taste good no more",
          cost: 8000,
          img: "Monkey14.jpg",
        },
        {
          name: "Monkey15",
          description: "Your Diaper Monkey",
          cost: 13000,
          img: "Monkey15.jpg",
        },
        {
          name: "Monkey16",
          description: "THe one and only sniper monkey",
          cost: 62000,
          img: "Monkey16.jpg",
        },
        {
          name: "Monkey17",
          description: "I don't play no games",
          cost: 53000,
          img: "Monkey17.jpg",
        },
        {
          name: "Monkey18",
          description: "I got a legendary pump shotgun",
          cost: 60000,
          img: "Monkey18.jpg",
        },
        {
          name: "Monkey19",
          description: "What gun do I have?",
          cost: 57000,
          img: "Monkey19.jpg",
        },
        {
          name: "Monkey20",
          description: "I will raid you; Professionally trained by cartels",
          cost: 100000,
          img: "Monkey20.jpg",
        },
        {
          name: "Monkey21",
          description: "🚬",
          cost: 50000,
          img: "Monkey21.jpg",
        },
        {
          name: "Monkey22",
          description: "Faded than a ho",
          cost: 100000,
          img: "Monkey22.jpg",
        },
        {
          name: "Monkey23",
          description: "Prisoner Monkey",
          cost: 1,
          img: "Monkey23.jpg",
        },
        {
          name: "Monkey24",
          description: "Faded than a ho",
          cost: 40000,
          img: "Monkey24.jpg",
        },
        {
          name: "Monkey25",
          description: "I will beat anyone up for u",
          cost: 200000,
          img: "Monkey25.jpg",
        },
        {
          name: "Monkey26",
          description: "I'm a thief",
          cost: 1000,
          img: "Monkey26.jpg",
        },
        {
          name: "Monkey27",
          description: "Leader of the Camorra",
          cost: 1000000,
          img: "Monkey27.jpg",
        },
      ],
    };
  },
};
</script>

<style>
.home {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-evenly;
}
.welcome {
  text-align: center;
}
</style>
