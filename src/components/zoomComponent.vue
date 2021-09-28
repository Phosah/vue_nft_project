<template>
  <div class="hello">
    <b-button-group class="zoom mt-10 mx-1" style="max-width: 148px; max-height: 49px">
      <b-button class="map">
        <img src="../assets/map.png">
      </b-button>
      <b-button class="line">
        <img src="../assets/line.png" class="line">
      </b-button>
      <b-button class="zoomOut">
        <img src="../assets/zoomOut.png">
      </b-button>
      <b-button class="zoomIn"> 
        <img src="../assets/zoomIn.png">
      </b-button>
    </b-button-group>
  </div>
</template>

<script>
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello .zoom{
  background-color:white;
  box-shadow: 0px 0px 16px rgba(90,90,90,0.16);
  border-radius: 8px;
}
.hello .zoom .map,
.hello .zoom .line,
.hello .zoom .zoomIn,
.hello .zoom .zoomOut
{
  background-color:#ffffff;
  color:black;
  border:none;
}
.hello .zoom .map img,
.hello .zoom .zoomIn img,
.hello .zoom .zoomOut img{
  width:24px;
  height:24px;
  padding:0.5px;
}
.hello .zoom .map:hover,
.hello .zoom .zoomIn:hover,
.hello .zoom .zoomOut:hover
{
  border:none;
}
</style>
