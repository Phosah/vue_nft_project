<template>
  <div class="home">
    <div class="mx-5 mx-auto">
      <div class="home-block d-flex">
        <section class="home-sidebar">
          Sidebar
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

export default {

}
</script>

<style scoped>
.home-block {
  background-color: aquamarine;
  height: 100vh;
}
.home-sidebar {
  background-color: bisque;
  width: 20%;
}
.home-navbar {
  background-color: sandybrown;
}
.home-main {
  background-color: silver;
  width: 80%;
}
.home-content {
  background-color: skyblue;
}
</style>