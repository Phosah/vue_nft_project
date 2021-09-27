<template>
  <div class="home text-white">
    <div class="container">
      <div class="home-block d-flex">
        <!-- Main Sidebar -->
        <section class="home-sidebar border-end border-white px-3">
          Sidebar
          <Collectibles />
        </section>
        <section class="home-main flex-grow-1">
          <nav class="home-navbar">Navbar</nav>
          <main class="home-content">Main</main>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
import Collectibles from '@/components/Collectibles'
export default {
  components: {
    Collectibles
  }
}
</script>

<style scoped>
.home-block {
  height: 100vh;
}
.home-sidebar {
  background-color: #222222;
}
.home-navbar {
  background-color: #222222;
}
.home-main {
  background-color: skyblue;
}
.home-content {
}
</style>