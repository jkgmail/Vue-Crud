<template>
<div id="ProductDisplay">

<div class="row">
<div class="col-md-6">
<h2><slot></slot></h2>
<ul>
<li v-for="product in products" v-on:click="productSelected = product">
{{ product.name }}: {{product.price}} Rs</li>
</ul>
</div>
<ProductDetail :product="productSelected"></ProductDetail>

</div>
</div>
</template>


<script>
import ProductDetail from './ProductDetail.vue'

export default{
name:'Products',
components:{
ProductDetail
},
data : function(){

return{
products : [
{name:'Product 1', price:100},
{name:'Product 2', price:200},
{name:'Product 3', price:300},
{name:'Product 4', price:100}
 ],
 productSelected:'Select a product'
}
}


}

</script>
