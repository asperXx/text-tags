<template>
  <v-app class="d-flex">
    <TextTags :cards="cards" />
  </v-app>
</template>

<script>
import TextTags from "./components/TextTags.vue";

export default {
  name: "App",

  components: {
    TextTags,
  },

  data: () => ({
    cards: [
      {
        title: "«Город сыра и мира»",
        tags: [
          {
            label: "5",
            icon: "mdi-star-outline",
          },
          {
            label: "Историческая",
          },
          {
            label: "На автобусе",
            icon: "mdi-bus",
          },
          {
            label: "25 марта",
          },
          {
            label: "9 часов",
            icon: "mdi-clock-outline",
          },
          {
            label: "до 49",
            icon: "mdi-account",
          },
        ],
      },
      {
        title: "Экскурсия в национальный парк «Куршская коса»",
        tags: [
          {
            label: "5",
            icon: "mdi-star-outline",
          },
          {
            label: "Обзорная",
          },
          {
            label: "На автобусе",
            icon: "mdi-bus",
          },
          {
            label: "26 марта",
          },
          {
            label: "9 часов",
            icon: "mdi-clock-outline",
          },
        ],
      },
      {
        title: "«О кирках, рыцарях и замках»",
        tags: [
          {
            label: "5",
            icon: "mdi-star-outline",
          },
          {
            label: "Историческая",
          },
          {
            label: "На автобусе",
            icon: "mdi-bus",
          },
          {
            label: "28 марта",
          },
          {
            label: "7 часов",
            icon: "mdi-clock-outline",
          },
          {
            label: "до 24",
            icon: "mdi-account",
          },
        ],
      },
      {
        title: "Экскурсия в Янтарный",
        tags: [
          {
            label: "Историческая",
          },
          {
            label: "На автобусе",
            icon: "mdi-bus",
          },
          {
            label: "29 марта",
          },
          {
            label: "5 часов",
            icon: "mdi-clock-outline",
          },
        ],
      },
    ],
  }),
};
</script>

<style lang="scss">
.main-container {
  border: 1px solid black;
  width: 60%;
  height: 100%;
  margin: 15px;
  align-self: center;
}
</style>
