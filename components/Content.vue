<template>
    <div v-if="isIndexRoute" class="content-container">
        <a href="#" class="alert-text">News and Insights</a>
       <h1>Latest Insights from Leading Voices</h1>
       <p>Solving the world’s problems through technology wouldn’t be possible without our most important invention: the NetSol. Have a look at our talented teams.</p>
       <a href="#" class="link-text">View All News</a>
    </div>
    <div  v-else class="content-container">
        <a href="#" class="alert-text">News and Insights</a>
       <h1>Latest Insights from {{ routeName }}</h1>
       <p>Solving the world’s problems through technology wouldn’t be possible without our most important invention: the NetSol. Have a look at our talented teams.</p>
       <a href="#" class="link-text">View All {{ routeName }} News</a>
    </div>
</template>

<script >
export default {
  computed: {
    isIndexRoute() {
      return this.$route.path === '/';
    },
    routeName() {
      return this.$route.name;
    }
  }
};
</script>

<style scoped>
.content-container{
    margin-top: 47px;
    text-align: center;
    padding:0 10px;
    /* border: 1px solid red; */
}
.alert-text{
    background: black;
    border-radius: 50px;
    padding: 11px 20px;
    font-size: 24px;
    line-height: 28.8px;
    border:1px solid #3d3d5ebe;
}
h1{
    font-size: 56px;
    line-height: 67.2px;
    margin-top: 20px;
}
p{
    margin: auto;
    font-size: 24px;
    line-height: 32px;
    margin-top: 10px;
    max-width: 1108px;
    margin-bottom: 20px;
    
}
.link-text{
    font-size: 16px;
    line-height:24px;
    text-decoration: underline;
    text-underline-offset: 0.3em; 
}
</style>

