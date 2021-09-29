<template>
  <div class="home">
    <div class="mx-5 mx-auto">
      <div class="home-block d-flex">
        <section class="home-sidebar">
          <div class="home-sidebar__logo-box d-flex align-items-center">
            <div class="me-2"><img src="../assets/logo.png" alt="Logo"></div>
            <div class="home-sidebar__logo-text fw-bold">QuestNFT</div>
          </div>
          <ArmyComponent />
          <Collectibles />
          <AllianceComponent />
        </section>
        <section class="home-main">
          <nav class="home-navbar">
          <Navbar />
          </nav>
          <main class="home-content">
            <ShowGeolocation />
            <Cards />
          </main>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
import ArmyComponent from "@/components/armyComponent"
import Collectibles from "@/components/Collectibles"
import Cards from '@/components/cards'
import Navbar from "../components/Navbar"
import AllianceComponent from "../components/AllianceComponent"
import ShowGeolocation from "../components/showGeolocation.vue"
export default {
  components: {
    ArmyComponent,
    Collectibles,
    Cards,
    Navbar,
    AllianceComponent,
    ShowGeolocation
  },
}
</script>

<style scoped>
.home-block {
  background-color: aquamarine;
  height: 100vh;
}
.home-sidebar {
  background-color: rgba(34, 34, 34, 1);
  width: 25%;
  padding: 20px;
  overflow-y: scroll;
}
.home-sidebar__logo-box {
  margin-bottom: 40px;
}
.home-sidebar__logo-text {
  font-size: 20px;
  color: #fff;
  letter-spacing: 0.3rem;
}
.home-sidebar::-webkit-scrollbar{
  width: 7px;
}
.home-navbar {
  border-left: 1px solid #A9A9A9;
}
.home-main {
  background-color: silver;
  width: 75%;
  position: relative;
}
.home-content {
  background-color: skyblue;
}
</style>