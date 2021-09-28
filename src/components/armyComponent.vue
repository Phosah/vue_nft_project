<template>
<div id="army-comp">
  
  <!-- <img src="../assets/armyComponent/caret.png" @click="showArmyMood" ref="caret" class="caret">
  <span class="army-heading">Army</span> -->

  <!-- Changes made here -->
  <div class="d-flex align-items-center my-2">
      <div @click="showArmyMood" class="me-2 caret" ref="caret"><img src="../assets/armyComponent/caret.png" alt="Arrow icon" ></div>
      <div class="army-heading">Army</div>
  </div>
  <!--  -->

  <div class="armyComp" v-if="showArmy">
    <div v-for="army in armies" v-bind:key="army.id" class="d-flex army align-items-center justify-content-between">
      <div class="rect-box d-flex justify-content-center align-items-center">
            <img :src="army.logo">
            <span>{{ army.value }}</span>
      </div>

      <div class="icon-img d-flex justify-content-between">
          <img :src="army.icon">
          <img :src="army.icon">
          <img :src="army.icon">
      </div>

      <span class="score">+{{ army.score }}</span>
    </div>
  </div>    
</div>
</template>

<script>
export default {
  name: "ArmyComponent",
  data() {
    return {
      showArmy: false,
      armies: [
        {
          id: 1,
          logo: require('@/assets/armyComponent/Vector1.png'),
          value: 500,
          icon: require('@/assets/armyComponent/imposter.png'),
          score: 3020
        },
        {
          id: 2,
          logo: require('@/assets/armyComponent/Vector2.png'),
          value: 100,
          icon: require('@/assets/armyComponent/purple-icon.png'),
          score: 300
        },
        {
          id: 3,
          logo: require('@/assets/armyComponent/Vector3.png'),
          value: 50,
          icon: require('@/assets/armyComponent/red-icon.png'),
          score: 300
        }
      ]
    }
  },
  methods: {
    showArmyMood(){
      this.showArmy = !this.showArmy
      this.$refs.caret.classList.toggle("rotate")
    }
  },
  watch: {
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Quattrocento+Sans:wght@700&display=swap');
#army-comp {
  color: #fff;
}

.army-heading {
  font-size: 14px;
  /* margin-left: 0.75rem; */
}

.armyComp {
  width: 100%;
  min-height: 142px;
  padding: 20px;
  background-color: #333333;
  font-family: 'Quattrocento Sans', sans-serif;
  border-radius: 6px;
}
.caret{
    transform: rotate(180deg);
  cursor: pointer;
}
.caret.rotate{
    transform: rotate(0deg);
}

.rect-box {
    width: 56px;
    height: 26px;
    border: 1px solid transparent;
    border-radius: 30px;
    font-size: 12px;
    background-image: linear-gradient(#333, #333), linear-gradient(45deg, #FC5C7D, #6A82FB);
    background-origin: border-box;
    background-clip: content-box, border-box;
}

/* .rect-box::before {
    content: '';
    position: absolute;
    border-radius: 30px;
    top: 0;
    right: 0;
    left: 0;
    bottom: 0;
    z-index: -5;
    margin: -1px;
    background: linear-gradient(to right, #FC5C7D, #6A82FB);

} */

.rect-box img {
  margin-right: 0.3125rem;
}

.army {
  margin-bottom: 0.8125rem;
}

.icon-img {
    width: 80px;
}

.score {
  font-size: 0.6875rem;
  width: 35px;
}
</style>