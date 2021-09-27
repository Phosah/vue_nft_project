<template>
    <div class="tooltip1">
      <span class="tooltiptext1">
        <div class="move">
          <div class="box3">
            <h3 class="text1">Lagoona</h3>
            <p class="text2">An Island in Lagos</p>
            <h3 class="text3">Description</h3>
            <p class="text4">
              A Demi God with great accomlishments siglehandedly winning the
              world war 4 by summoning his Infinite troops
            </p>
          </div>
          <div class="box5">
            <h3 class="text5">Location Health</h3>
            <div class="box4">
              <p class="text6">60%</p>
              <!-- <i class="fas fa-battery-three-quarters"></i> -->
              <div class="battery">
                <div class="battery-level"></div>
              </div>
            </div>

            <h3 class="text8">Attributes</h3>
            <div class="box6">
              <div>
                <i class="icon ms-3 fas fa-fire"></i>
              </div>
              <div class="text7 product ms-4">Power NFTs</div>
              <div class="text9 product ms-4">80xp</div>
            </div>
            <div class="box6">
              <div>
                <i class="icon ms-3 fas fa-fire"></i>
              </div>
              <div class="text7 product ms-4">Agility</div>
              <div class="text10 product ms-4">22xp</div>
            </div>
            <div class="box6">
              <div>
                <i class="icon ms-3 fas fa-fire"></i>
              </div>
              <div class="text7 product ms-4">Speed</div>
              <div class="text11 product ms-4">15xp</div>
            </div>
            <div class="box6">
              <div>
                <i class="icon ms-3 fas fa-fire"></i>
              </div>
              <div class="text7 product ms-4">Pet</div>
              <div class="text12 product ms-4">39xp</div>
            </div>
          </div>
        </div>
      </span>
    </div>
</template>
<script>
export default {
    name: 'Tooltip1',
};
</script>


 <style scoped>
      .tooltip1 {
        position: relative;
        display: inline-block;
        margin-top: 400px;
        margin-left: 100px;
      }

      .tooltip1 .tooltiptext1 {
        /* visibility: hidden; */
        height: 370px;
        width: 500px;
        background-color: rgba(26, 25, 25, 1);
        color: #fff;
        border-radius: 12px;
        position: absolute;
        z-index: 1;
        bottom: 150%;
        left: 50%;
        margin-left: -60px;
        padding: 0px 30px;
      }

      .tooltip1 .tooltiptext1::after {
        content: "";
        position: absolute;
        top: 100%;
        left: 50%;
        margin-left: -5px;
        border-width: 13px;
        border-style: solid;
        border-color: rgba(26, 25, 25, 1) transparent transparent transparent;
      }

      /* .tooltip1:hover .tooltiptext1 {
        visibility: visible;
      } */
      .box3 {
        height: 310px;
        width:40%;
       
       
      }
      .box5 {
        height: 310px;
        width: 50%;
      margin-left: 50px;
       
      }
      .text1 {
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: bold;
        font-size: 22px;
        line-height: 12px;
        margin-top: 50px;
        color: #ffffff;
      }
      .text2 {
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: normal;
        font-size: 21px;
        line-height: 9px;
        color: #c4c4c4;
      }
      .text3 {
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: bold;
        font-size: 22px;
        line-height: 12px;
        color: #ffffff;
        margin-top: 40px;
      }
      .text4 {
        
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: normal;
        font-size: 21px;
        line-height: 24px;
        color: #c4c4c4;
        height: 145px;  
      }
      .text5 {
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: bold;
        font-size: 22px;
        line-height: 12px;
        margin-top: 50px;
        color: #ffffff;
        margin-left: 95px;
      }
      .text6 {
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: normal;
        font-size: 21px;
        line-height: 9px;
        color: #c4c4c4;
      }
      .move {
        display: flex;
        justify-content: center;
        border-bottom: 0.7px solid white;
      }
      .battery {
        border: 3px solid #333;
        width: 55px;
        height: 16px;
        padding: 2px;
        border-radius: 4px;
        position: relative;
        margin: 15px 0;
        margin-left: 20px;
      }

      .battery-level {
        background: linear-gradient(90deg, #fc5c7d 0%, #6a82fb 100%);
        height: 85%;
        width: 60%;
        position: absolute;
        margin-left: 23px;
      }
      .box4 {
        display: flex;
        margin-top: -20px;
        margin-left: 125px;
      }

      .box6 {
        display: flex;
        line-height: 33px;
        margin-left: 35px;
      }
      .icon {
        font-size: 20px;
        background-color: radial-gradient(
          75.02% 96.52% at 48.12% 100.26%,
          #ff9800 31.4%,
          #ff6d00 66.2%,
          #f44336 97.2%
        );
        margin-left: 10px;
      }
      .icon1 {
        font-size: 20px;
        color: rgba(97, 96, 97, 1);
      }
      .text7 {
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: normal;
        font-size: 21px;
        line-height: 23px;
        color: #c4c4c4;
        margin-left: 15px;
      }
      .text8 {
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: bold;
        font-size: 22px;
        line-height: 12px;
        color: #ffffff;
        margin-left: 35px;
      }
      .text9 {
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: bold;
        font-size: 22px;
        line-height: 12px;
        color: #ffffff;
        margin-top: 5px;
        margin-left: 18px;
      }
      .text10 {
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: bold;
        font-size: 22px;
        line-height: 12px;
        color: #ffffff;
        margin-top: 5px;
        margin-left: 64px;
      }
      .text11 {
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: bold;
        font-size: 22px;
        line-height: 12px;
        color: #ffffff;
        margin-top: 5px;
        margin-left: 70px;
      }
      .text12 {
        font-family: Quattrocento Sans;
        font-style: normal;
        font-weight: bold;
        font-size: 22px;
        line-height: 12px;
        color: #ffffff;
        margin-top: 5px;
        margin-left: 94px;
      }
      
    </style>