<template>
  <div>
    <b-row>
      <b-col cols="12" xs="2" md="3" v-for="(item, index) in pool" :key="index">
        <nft-card />
      </b-col>
    </b-row>
  </div>
</template>

<script>
import nftCard from "../components/nftCard.vue";

export default {
  name: "cardGrid",
  components: {
    nftCard,
  },
  data() {
    return {
      pool: [
        {
          name: "Power Stone",
          image: "./images/nftimg.jpeg",
        },
        {
          name: "Power Stone",
          image: "./images/nftimg.jpeg",
        },
        {
          name: "Power Stone",
          image: "./images/nftimg.jpeg",
        },
        {
          name: "Power Stone",
          image: "./images/nftimg.jpeg",
        },
        {
          name: "Power Stone",
          image: "./images/nftimg.jpeg",
        },
        {
          name: "Power Stone",
          image: "./images/nftimg.jpeg",
        },
        {
          name: "Power Stone",
          image: "./images/nftimg.jpeg",
        },
        {
          name: "Power Stone",
          image: "./images/nftimg.jpeg",
        },
      ],
    };
    },
};
</script>

<style scoped>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
