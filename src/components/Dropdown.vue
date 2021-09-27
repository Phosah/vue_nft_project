<template>
  <div @click="isDropDown = false">
   <svg width="14" height="4" viewBox="0 0 14 4" fill="none" xmlns="http://www.w3.org/2000/svg" @mouseover="isDropDown = true">
    <path d="M2.04346 0.394531C1.15105 0.394531 0.420898 1.12469 0.420898 2.01711C0.420898 2.90953 1.15105 3.63969 2.04346 3.63969C2.93587 3.63969 3.66602 2.90953 3.66602 2.01711C3.66602 1.12469 2.93587 0.394531 2.04346 0.394531ZM11.7788 0.394531C10.8864 0.394531 10.1563 1.12469 10.1563 2.01711C10.1563 2.90953 10.8864 3.63969 11.7788 3.63969C12.6712 3.63969 13.4014 2.90953 13.4014 2.01711C13.4014 1.12469 12.6712 0.394531 11.7788 0.394531ZM6.91114 0.394531C6.01873 0.394531 5.28858 1.12469 5.28858 2.01711C5.28858 2.90953 6.01873 3.63969 6.91114 3.63969C7.80354 3.63969 8.53369 2.90953 8.53369 2.01711C8.53369 1.12469 7.80354 0.394531 6.91114 0.394531Z" fill="white"/>
  </svg>
  <div class="dropdown" v-if="isDropDown">
    <ul>
      <li>Purchase</li>
      <li>Sell as NFT</li>
      <li>Boost Troop</li>
      <li class="last">Share </li>
    </ul>
  </div>
  </div>
</template>

<script>
export default {
    data () {
        return {
            isDropDown: false
        }
    }
}
</script>

<style scoped>
svg{
    position:relative;
    height:25px;
    width:15px;
    margin-bottom:0px;
}
.dropdown{
    position:absolute;
    width: 125.95px;
    height: 155.82px;
    background-color:black;
    color:white;
    transition:  0.5s ease-in-out;
}
ul{
    display:flex;
    flex-direction:column;
    justify-content: space-evenly;
    width:100%;
    height:100%;
    align-items: center;
    text-align:center;
    margin:0;
    padding:0;
    line-height:16.32px;
    font-size:12.71px;
}
li{
    border-bottom: 0.847395px solid #333333;
    width:100%;
    padding:5px;
    padding-bottom:8px;
}
.last{
    border-bottom:none;
    padding-bottom:5px;
}
li:hover{
    color:red;
}
</style>