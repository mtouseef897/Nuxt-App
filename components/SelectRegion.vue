<template>
    <div>
      <button @click="toggleDropdown" class="region-btn">Regions</button>
      <div v-if="showDropdown" class="dropdown">
        <ul>
            <li><NuxtLink to="/en-us">USA</NuxtLink></li>
            <li><NuxtLink to="/en-uk">UK</NuxtLink></li>
            <li><NuxtLink to="/en-cn">China</NuxtLink></li>
            <li><NuxtLink to="/en-pk">Pakistan</NuxtLink></li>
        </ul>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        showDropdown: false,
        selectedRegion: null
      };
    },
    methods: {
      toggleDropdown() {
        this.showDropdown = !this.showDropdown;
      }
    }
  };
  </script>
  
  <style>

.region-btn{
    font-size: 16px;
    font-family: 'Aeonik Regular';
    line-height: 19.2px;
    padding: 10px 50px;
    border-radius: 100px;
    color: white;
    background:  radial-gradient(rgba(0, 37, 206, 1),rgba(9, 93, 230, 0.53));
    box-shadow: inset 0px 9px 15px 0px rgba(13, 147, 239, 1);
    border: 1px solid white; 
    cursor: pointer;
  }
  
  .dropdown {
    margin-top: 5px;
    right: 1%;
    position: absolute;
    background: #092530;
    padding: 35px 34px;
    width: 268px;
    height: 268px;
    border-radius: 15px ;
    border: 0.5px solid white;
  }

  li{
    padding: 4px;
    border-bottom: 0.5px solid white;
    margin-bottom: 21px;
  }

  .router-link-active{
    color: #00EAFF;
  }
 
  </style>
  