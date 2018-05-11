<template>
<div id="TitleBar">
<h1>{{Title}}</h1>
</div>
</template>


<script>
export default {
  name: 'TitleBar',
  props:{
  Title : String
  }
}
</script>


<style>
#TitleBar {
  text-align:center;
}
</style>
