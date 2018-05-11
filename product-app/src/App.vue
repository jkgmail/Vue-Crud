<template>
  <div id="app">
  <TitleBar Title="Product Application"></TitleBar>
  <Products>Products Available</Products>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import TitleBar from './components/TitleBar.vue'
import Products from './components/ProductsDisplay.vue'

export default {
  name: 'app'
  ,components: {
    HelloWorld,
    TitleBar,
    Products
  }

}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
