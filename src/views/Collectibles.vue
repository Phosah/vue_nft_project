<template>
  <div class="home">
    <div class="mx-5 mx-auto">
      <section class="home-main">
        <header>
            <div class="header">

          <CollectibleNavbar />
            </div>
        </header>
        <main class="home-content">
          <div class="content">
            <NftCard v-for="n in 5" :key="n" />
          </div>
        </main>
      </section>
    </div>
  </div>
</template>

<script>
import CollectibleNavbar from "../components/collectibleNavbar.vue";
import NftCard from "../components/nftCard.vue";
export default {
  components: {
    CollectibleNavbar,
    NftCard,
  },
};
</script>

<style scoped>
.home{
  height: 100vh;
  background: #222222;
}
.home-main {
  width: 100%;
  position: relative;
}
.content {
  display: grid;
  padding: 30px;
  grid-template-columns: repeat(4, 1fr);
  grid-column-gap: 20px;
}
</style>