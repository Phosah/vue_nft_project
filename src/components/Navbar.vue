<template>
  <div class="navbar d-flex flex-nowrap align-items-center justify-content-between px-4">
    <div class="d-flex align-items-center">
      <div class="navbar-title me-3">Ongoing Battles</div>
      <div class="d-flex align-items-center">
        <div>
          <div>
            <img src="../assets/eugene-logo.png" alt="kayla-logo">
          </div>
          <div class="navbar-player">Eugene</div>
        </div>
        <!--  -->
        <div class="mx-2">
          <div>
            <img src="../assets/emojione_crossed-swords.png" alt="emojione_crossed-swords-logo">
          </div>
        </div>
        <!--  -->
        <div class="me-2">
          <img src="../assets/kayla-logo.png" alt="kayla-logo-logo">
          <div class="navbar-player">Kayla</div>
        </div>
        <!--  -->
        <div>
          <img src="../assets/arrow-down.png" alt="arrow-down">
        </div>
      </div>
    </div>
    <div class="mx-1">
      <SearchBox @handleSearch="Search($event)"/>
    </div>
    <div class="d-flex align-items-center me-1">
      <div>
        <img src="../assets/noto_coin.png" alt="noto_coin-logo">
      </div>
      <div class="navbar-coins me-3">320</div>
      <div class="">
        <img src="../assets/eugene-lg-logo.png" alt="eugene-lg-logo-logo">
      </div>
    </div>
  </div>
</template>

<script>
import searchBox from "@/components/searchBox.vue";
export default {
  name: "Navbar",
  components: {
    searchBox
  },
  data(){
    return {
      search: ""
    }
  },
  methods: {
    Search(search){
      this.search = search
    }
  }
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Quattrocento+Sans:wght@700&display=swap');

.navbar {
  height: 67px;
  background: #222222;
  color: #fff;
}
.navbar-title {
  font-size: 14px;
  font-family: 'Quattrocento Sans', sans-serif;
}
.navbar-player {
  font-size: 10px;
  font-family: 'Quattrocento Sans', sans-serif;
}
</style>