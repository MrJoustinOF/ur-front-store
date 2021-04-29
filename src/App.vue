<template>
  <div id="nav">
    <h1><router-link to="/">urFrontStore</router-link></h1>
    <ul class="itemsMenu">
      <li><router-link to="/">Home</router-link></li> 
      <li><router-link to="/about">About</router-link></li>
    </ul>
    <span class="btn_menu">
      <img src="https://github.com/MrJoustinOF/Responsive-Fixed-Top-Navbar/blob/master/img/btnMenu.png?raw=true" 
      v-on:click="mostrarMenu"
      >
    </span>
  </div>  
  <div class="data">
    <router-view/>
  </div>
</template>

<script>
  export default {
    methods:{
      mostrarMenu: () => {
        const menu_items = document.querySelector('.itemsMenu')
        menu_items.classList.toggle('show')
      } 
    }  
  }
</script>

<style src="./assets/css/style.css">

</style>
