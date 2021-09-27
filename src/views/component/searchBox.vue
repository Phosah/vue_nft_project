<template>
  <div class="searchBox">
    <h1>Search Component</h1>
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

input{
  border: 1px solid grey;
  border-radius: 5px;
  height: 30px;
  width:400px;
  margin: 40px;
  outline: 0;
  font-size: 15px;
  padding: 6px;
  background-color: #f5f5f5;
  float:right;
}
input:hover, input:focus{
  border : 2px solid blue;
  background-color: white;
}
h3{
  float: right;
  font-size: 20px;
  text-align: center;
  margin: 40px;
  top:0px;
}
</style>
