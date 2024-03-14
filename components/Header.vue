<template>
    <div>
        <header>
           <NuxtLink to="/"> <img src="/images/logo.png" alt="Logo image"></NuxtLink>
            <SelectRegion/>
        </header>
    </div>
</template>

<script setup>

</script>

<style  scoped>
 header{
    padding: 0 92px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 83px;
    /* border: 1px solid green; */
    /* border-bottom: 1px solid rgba(255, 255, 255, 0.1); */
    border-bottom: 1px solid;
  border-image: radial-gradient( #9b97978c, #55627000); /* Adjust gradient colors and direction as needed */
  border-image-slice: 1; 
;
  }

  .region-btn{
    font-size: 16px;
    font-family: 'Aeonik Regular';
    line-height: 19.2px;
    padding: 10px 50px;
    border-radius: 100px;
    color: white;
    background:  radial-gradient(rgba(0, 37, 206, 1),rgba(9, 93, 230, 0.53));
    box-shadow: inset 0px 9px 15px 0px rgba(13, 147, 239, 1);
    border: 1px solid white; /* Set the border width and make it transparent */
  }
</style>