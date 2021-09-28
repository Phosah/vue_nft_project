<template>
  <div class="m-3">
    <b-row>
      <b-col class="blackMe">
        <p class="elli mx-1">...</p>
        <img
          style="width: 100%"
          src="../assets/nftimg.jpeg"
          alt=""
          class="py-2"
        />
        <b-row class="my-2 mx-0 p-0">
          <b-row class="gutt" align-h="between">
            <b-col class="p-0 m-0">
              <span class="whiteThis p-0 m-0">Power Stone</span>
            </b-col>

            <b-col class="testing">
              <button size="sm" class="mx-1 butt">🔥 24</button>
              <button size="sm" class="mx-1 butt">⚡ 24</button>
            </b-col>
          </b-row>

          <p class="my-3 px-0 py-2 subp">
            Power StonePower StonePower StonePower StonePower StonePower
            StonePower StonePower StonePower Stone...
          </p>
        </b-row>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  name: "nftCard",
  
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.testing {
  display: flex;
  justify-content: flex-end;
}

.whiteThis {
  color: white;
  text-align: start;
  font-size: 1.2rem;
  font-weight: 500;
}
.elli {
  text-align: end;
  color: white;
  font-size: 1.3rem;
}
.blackMe {
  background-color: #333232 !important;
}
.subp {
  color: grey;
  font-size: 0.7rem;
  text-align: start;
}
.butt {
  border-radius: 10px !important;
  background-color: #404141;
  color: white;
  border: 1px solid #404141;
  font-size: 10px;
  width: 50px;
  height: 25px;
}

.gutt {
  --bs-gutter-x: 0;
}
</style>
