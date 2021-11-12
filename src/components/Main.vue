<template>
  <div class="main-container">
    <div class="top-black">
      <CardsSection></CardsSection>
    </div>
    <div class="bottom-blue">
      <div class="flex">
        <div
          class="card-container"
          v-for="(chiave, i) in imgBlueContainer"
          :key="i"
        >
          <img :src="chiave.src" alt="" />
          <span>{{ chiave.description }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import cardsContainer from "@/components/CardsSection.vue";
import CardsSection from "../components/CardsSection.vue";
export default {
  components: { CardsSection },
  name: "Main",
  data() {
    return {
      imgBlueContainer: [
        {
          src: require("../assets/buy-comics-digital-comics.png"),
          description: "DIGITAL COMICS",
        },
        {
          src: require("@/assets/buy-comics-merchandise.png"),
          description: "DC MERCHANDISE",
        },
        {
          src: require("../assets/buy-comics-subscriptions.png"),
          description: "SUBSCRIPTION",
        },
        {
          src: require("../assets/buy-comics-shop-locator.png"),
          description: "COMIC SHOP LOCATOR",
        },
        {
          src: require("../assets/buy-dc-power-visa.svg"),
          description: "DC POWER VISA",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../styles/main.scss";
</style>