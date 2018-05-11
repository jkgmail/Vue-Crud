<template>
<div>
<h2><slot></slot></h2>
<ul>
<li v-for="product in products">
{{ product.name }}: {{product.price}} Rs</li>

</ul>
</div>
</template>


<script>
export default{
name:'Products',
data : function(){

return{
products : [
{name:'Product 1', price:100},
{name:'Product 2', price:200},
{name:'Product 3', price:300},
{name:'Product 4', price:100}

 ]
}
}
}
</script>
