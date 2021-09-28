<template>
  <div class="navbar">
    <div class="navbarLeft">
      <h3>Ongoing Battles</h3>
      <div class="navbarlogos">
        <div class="navbarlogo">
          <img src="../assets/eugene-logo.png" alt="kayla-logo">
          <h5>Eugene</h5>
        </div>
        <div class="navbarlogo">
          <img src="../assets/emojione_crossed-swords.png" alt="emojione_crossed-swords-logo">
        </div>
         <div class="navbarlogo">
          <img src="../assets/kayla-logo.png" alt="kayla-logo-logo">
          <h5>Kayla</h5>
        </div>
        <div class="navbarlogo">
          <img src="../assets/arrow-down.png" alt="arrow-down">
        </div>
      </div>
    </div>
    <div class="navbarRight">
      <searchBox @handleSearch="Search($event)"/>
      <div class="navbarlogo__1">
        <img src="../assets/noto_coin.png" alt="noto_coin-logo">
        <h3>320</h3>
      </div>
      <div class="navbarlogo__1">
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
.navbar {
  width: 100%;
  height: 67px;
  background: #222222;
  padding: 16px ;
  box-sizing: border-box;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  overflow: hidden;
  flex-wrap: nowrap;
}

.navbarLeft {
  position: relative;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  margin-left: 1rem;
}
.navbarLeft h3 {
  color: white;
  font-size: 14px;
  font-weight: 500;
  font-family: Quattrocento Sans;
  margin-right: 1rem;
}
.navbarlogos {
  display: flex;
  flex-direction: row;
  padding: 0.7rem 0.4rem;
}

.navbarlogo {
  margin-left: 0.3rem;
  justify-content: center;
  align-items: center;
  display: flex;
  flex-direction: column;
}
.navbarlogo:nth-child(2) {
  margin-top: 0.1rem;
}
.navbarlogo img {
  margin: 0.2rem;
}
.navbarlogo h5 {
  color: white;
   font-size: 8px;
   font-weight: 200;
  font-family: Quattrocento Sans;
}
.navbarRight {
  justify-content: center;
  align-items: center;
  display: flex;
  flex-direction: row;
}
.navbarlogo__1:nth-child(1) {
  margin-left: 2rem;
}
.navbarlogo__1:nth-child(2) {
  display: flex;
  flex-direction: row;
  margin-right: 1rem;
}
.navbarlogo__1:nth-child(2) h3 {
  color: white;
  font-size: 14px;
  font-weight: 300;
  font-family: Quattrocento Sans;
}
.navbarlogo__1:nth-child(2) img {
  font-size: 30px;
  margin-right: 0.5rem;
  width: 100%;
  height: 100%;
}
.navbarlogo__1:nth-child(3) {
  margin-right: 2rem;
}
</style>