<template>
  <div class='container'>
    <div class='card-1'>
        <img src="@/assets/vello.png" alt="">
      <div class="text-container"><span class="big-font" style="font-weight: bold; font-size: 14px; line-height: 20px">Vello</span>
      <span class="info">!</span><br>
      <span style="line-height: 0px">Demon Slayer</span>
      </div>
    </div>

    <div class='card-2'>
      <img src="@/assets/kayla.png" alt="">
      <div class= "text-container small kayla"><span class= "big-font">Kayla</span><br><span>Seeker</span></div>
    </div>

    <div class='card-3'>
      <img src="@/assets/darth.png" alt="" >
    <div class= "text-container small"><span class= "big-font">Darth</span><br><span>Soldier</span></div>
    </div>
  </div>
</template>

<script>

export default{};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.container {
  background: transparent;
  box-sizing: border-box;
  position: absolute;
  bottom: 30px;
  left: 0;
  width: 203px;
  height: 151.01px;
}
.card-1 {
  position: absolute;
  width: 106.45px;
  height: 150.01px;
  top: 50%;
  left: 50%;
  z-index: 1;
  transform: translate(-50%, -50%);
  background: linear-gradient(90deg, #EC008C 0%, #FC6767 100%);
  border: 2.47561px solid rgba(230, 230, 230, 0.46);
  border-radius: 9.90244px;
}
.card-2 {
  position: absolute;
  width: 83.49px;
  height: 118.44px;
  top:10%;
  background: linear-gradient(90deg, #A73737 0%, #7A2828 100%);
  border: 1.94165px solid rgba(230, 230, 230, 0.46);
  border-radius: 7.76662px;
}
.card-3  {
  position: absolute;
  width: 83.49px;
  height: 118.44px;
  margin-left: 57%;
  top:10%;
  background: linear-gradient(90deg, #4776E6 0%, #8E54E9 100%);
  border: 1.94165px solid rgba(230, 230, 230, 0.46);
  border-radius: 7.76662px;
}
img{
  position: relative;
  top: 10px;
}
.text-container{
  width: 106.45px;
  height: 38.37px;
  margin-top: 19px;
  border-bottom-left-radius: 7.76662px;
  border-bottom-right-radius: 7.76662px;
  text-align: center;
  color: white;
  font-family: Neue Helvetica;
  font-style: normal;
  font-weight: normal;
  font-size: 8.66463px;
  line-height: 168%;
  background: red;
}
.small{
  width: 83.49px;
  height: 27px;
  background: blue;
  border-radius: 0px 0px 9.14776px 7.91997px;
  line-height: 10px;
  font-family: Neue Helvetica;
  font-style: normal;
  font-weight: normal;
  font-size: 8.66463px;
  color: white;
}
.kayla{
  background-color: rgb(110, 34, 34);
}
.big-font{
  font-family: Neue Helvetica;
  font-style: normal;
  font-weight: bold;
  font-size: 9.70827px;
  z-index: 5;
  color: #E6E6E6;
  mix-blend-mode: normal;
}
.info{
  background-color: white;
  position: relative;
  font-weight: bold;
  font-size: 10px;
  color: rgba(248, 72, 114, 1);
  top: -11px;
  padding: 2px 4px;
  left: 17px;
  border-radius: 50%;
}
</style>
