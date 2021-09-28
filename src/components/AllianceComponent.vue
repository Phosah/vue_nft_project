<template>
  <div id="alliance-comp">
    <div class="d-flex justify-content-between my-2">
        <div class="d-flex align-items-center">
            <div @click="showAllianceMood" class="me-2 caret" ref="caret"><img src="@/assets/allianceComponent/caret.png" alt="Arrow icon" ></div>
            <div class="alliance-heading">Alliance</div>
        </div>
        <div><img src="@/assets/dots.png" alt="Dot icon"></div>
    </div>

    <div class="allianceComp" v-if="showAlliance">
      <div class="mb-3 d-flex justify-content-start">
        <img class="" src="@/assets/allianceComponent/group-0.png" />
        <img
          class="ms-1"
          src="@/assets/allianceComponent/emojione_handshake-1.png"
        />
        <img class="ms-1" src="@/assets/allianceComponent/group-1.png" />
      </div>
      <div
        v-for="alliance in alliances"
        v-bind:key="alliance.id"
        class="alliance-block fw-bold d-flex alliance align-items-center justify-content-between"
      >
        <div>
          <span>{{ alliance.name }} </span>

          <img :src="alliance.icon" />
        </div>

        <span>{{ alliance.value }}</span>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  data() {
    return {
      showAlliance: true,
      alliances: [
        {
          id: 1,
          name: "Global Ranking",
          icon: require("@/assets/allianceComponent/vector-1.png"),
          value: "#23",
        },
        {
          id: 2,
          name: "Cities Controlled",
          icon: require("@/assets/allianceComponent/vector-2.png"),
          value: "21 Cities",
        },
      ],
    };
  },
  methods: {
    showAllianceMood() {
      this.showAlliance = !this.showAlliance;
      this.$refs.caret.classList.toggle("rotate");
    },
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Quattrocento+Sans:wght@700&display=swap");
#alliance-comp {
  color: #fff;
}

.alliance-heading {
  font-size: 14px;
}
.caret{
  transform: rotate(0deg);
  cursor: pointer;
}
.caret.rotate{
  transform: rotate(180deg);
}

.allianceComp {
  width: 100%;
  min-height: 142px;
  padding: 20px;
  background-color: #333333;
  font-family: "Quattrocento Sans", sans-serif;
  border-radius: 6px;
}

.alliance {
  margin-bottom: 0.8125rem;
}

.value {
  /* font-size: 0.6875rem; */
  /* margin-right: 21px; */
}
.alliance-block {
  font-size: 14px;
}
</style>