<template>
    <div class="blog-card-container">
        <BlogCard v-for="product in products" :key="product.title" :product="product" />
    </div>
</template>

<script>
import products from '~/data.js'; // Import the products data file
export default {
  data() {
    return {
      products: products, // Assign the imported products array to the component's data
    };
  },
};
</script>

<style scoped>
.blog-card-container{
 /* border: 1px solid red; */
  display:flex;
  justify-content:center;
  flex-wrap: wrap;
  max-width: 1736px;
  margin: auto;
  margin-top: 81px;
  gap: 30px;
}
</style>

