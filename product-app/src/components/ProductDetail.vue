<template>
<div id="ProductDetail" class="col-md-6">
<h2>Edit Product</h2>
<div v-if="product.name">
<input type="text" v-model="product.name"></input>
<input type="text" v-model="product.price"></input>
</div>
<div v-else>
Please click on a product to edit
</div>
</div>
</template>

<script>
export default{
name:'ProductDetail',
props:{
product : {}
}}
</script>
