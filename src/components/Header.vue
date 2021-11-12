<template>
  <div class="header-container">
    <img alt="Vue logo" src="../assets/dc-logo.png" class="logo" />
    <ul>
      <li v-for="(key, i) in headerItems" :key="i">
        {{ key.titolo }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      headerItems: [
        {
          titolo: "Characters",
        },
        {
          titolo: "Comics",
        },
        {
          titolo: "Movies",
        },
        {
          titolo: "TV",
        },
        {
          titolo: "Games",
        },
        {
          titolo: "Collectibles",
        },
        {
          titolo: "Videos",
        },
        {
          titolo: "Fans",
        },
        {
          titolo: "News",
        },
        {
          titolo: "Shop",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../styles/header.scss";
</style>