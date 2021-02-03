<template>
  <div id="app">

    <card v-for="(card, idx) in cards" :key="card.title">
      <template #header>
        <h1 v-if="idx != 0">{{ card.title }}</h1>
      </template>
      <template #default>
        <p v-if="idx != 1" :style="`color: ${card.color}`">{{ card.text }}</p>
      </template>
    </card>
    
  </div>
</template>

<script>
import Card from "./components/Card";

export default {
  components: {
    Card
  },
  data() {
    return {
      cards: [
        {
          title: "Card 1",
          text: "Text for the Card 1",
          color: "red",
        },
        {
          title: "Card 2",
          text: "Text for the Card 2",
          color: "green",
        },
        {
          title: "Card 3",
          text: "Text for the Card 3",
          color: "blue",
        }
      ]
    }
  },
}
</script>
