<template>
  <div class="hello">
    <b-list-group horizontal style="max-width: 640px; max-height: 44px" class="CollectibleNav">
      <b-list-group-item class="all">All</b-list-group-item>
      <b-list-group-item class="art">Artifacts</b-list-group-item>
      <b-list-group-item class="terr">Territories</b-list-group-item>
      <b-list-group-item class='army'>Armies</b-list-group-item>
    </b-list-group>
  </div>
</template>

<script>
export default {
  name: "HelloWorld"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.hello .CollectibleNav{
  font-size:14px;
  padding:0px;
  margin-left:40px;
}
.hello .CollectibleNav .all,
.hello .CollectibleNav .art,
.hello .CollectibleNav .terr,
.hello .CollectibleNav .army{
  width:160px;
  height:44px;
  background-color:#333333;
  color:#808080;
}
.hello .CollectibleNav .all,
.hello .CollectibleNav .art,
.hello .CollectibleNav .terr,
.hello .CollectibleNav .army{
  border-bottom:1px solid #808080;
  border-top:1px solid #808080;
}
.hello .CollectibleNav .all,
.hello .CollectibleNav .art,
.hello .CollectibleNav .terr,
.hello .CollectibleNav .army{
  border-left:1px solid #808080;
}
.hello .CollectibleNav .army{
  border-right:1px solid #808080;
}
.hello .CollectibleNav .all:hover,
.hello .CollectibleNav .art:hover,
.hello .CollectibleNav .terr:hover,
.hello .CollectibleNav .army:hover
{
  background-color:white;
  color:black;
  border: none;
}
</style>
