<template>
  <div class="home">
    <div class="mx-5 mx-auto">
      <div class="home-block d-flex">
        <section class="home-sidebar">
          <ArmyComponent />
          <Collectibles />
        </section>
        <section class="home-main">
          <nav class="home-navbar">Navbar</nav>
          <main class="home-content">Main</main>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
import ArmyComponent from "@/components/armyComponent.vue"
import Collectibles from "@/components/Collectibles.vue"
export default {
  components: {
    ArmyComponent,
    Collectibles
  }
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
  padding: 30px;
}
.home-navbar {
  background-color: sandybrown;
}
.home-main {
  background-color: silver;
  width: 75%;
}
.home-content {
  background-color: skyblue;
}
</style>