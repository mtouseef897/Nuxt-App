<template>
    <div class="blog-card">
        <img :src="product.image" alt="Services-Featured-Image">
        <p class="tag">{{ product.tag }}</p>
        <h2>{{ product.title }}</h2>
        <p class="brief">{{ product.brief }}</p>
    </div>
</template>

<script >
export default {
  props: {
    product: Object, // Prop to receive the product object
  },
};
</script>
<style>
.blog-card{
  max-width: 409px;
}

img{
  max-width: 404px;
}
.brief{
  font-size: 18px;
  line-height: 26px;
  margin-top: 10px;
  font-weight: 400;
}
.tag{
  color:#18EBFE;
  padding: 6px 10px;
  background: rgba(255, 255, 255, 0.1);
  border-radius: 5px;
  display: inline-block;
  margin-top: 20px;
}

h2{
  font-size: 24px;
  line-height: 30px;
  margin-top: 16px;
}


</style>

