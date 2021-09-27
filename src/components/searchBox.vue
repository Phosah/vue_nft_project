<template>
  <div class="searchBox">
    <input type="text" placeholder="Search Cities, Players and Nfts etc." v-model= "search" :class= "search" model-event = "Change">
    <h3>{{search}}</h3>
  </div>
</template>

<script>
  //import { ref } from '@vue/composition-api'
  export default {
  name: 'SearchBox',
  props: {
  },
  //setup(){
    //const search= ref(null)

    //const handleChange = ()=>{
      //search.value = " "
    //}
    //return {search, handleChange, ref}
  //}
  data(){
    return{
      search: " "
    }
  },
  methods: {
    handleChange(){
      this.$ref.search.value
    }
  },
}
</script>

<style scoped>
.searchBox{
  position: absolute;
  left: 45%;
  top: 7%;
  box-sizing: border-box;
}
input{
  border: 3px solid #eee;
  border-radius: 10px;
  height: 41px;
  width:400px;
  outline: none;
  border: none;
  font-size: 15px;
  padding: 0 20px;
  background-color: #333333;
  margin-top: 0.5rem;
  align-items: center;
  color: #eee;
}
.search::placeholder {
color: #eee;
}
input:hover, input:focus{
  outline: none;
  border: none;
  background-color: white;
  color: #333333;
}
h3{
  float: right;
  font-size: 20px;
  text-align: center;
  margin: 40px;
  top:0px;
}
</style>
