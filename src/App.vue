<template>
  <div id="app">
    <HeaderComponent></HeaderComponent>
    <Slider></Slider>
    <div class="center">
      <!-- <LastArticles></LastArticles> -->
      <router-view></router-view>
      <SideBar></SideBar>
      <div class="clearfix"></div>
    </div>
    <FooterComponent></FooterComponent>
    
  </div>
</template>

<script>
/* eslint-disable */
import HelloWorld from './components/HelloWorld.vue'
import MiComponente from './components/MiComponente.vue'
import HeaderComponent from './components/HeaderComponent.vue'
import Slider from './components/Slider'
import SideBar from './components/SideBar.vue'
import LastArticles from './components/LastArticles.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    MiComponente,
    HeaderComponent,
    Slider,
    SideBar,
    LastArticles,
    FooterComponent
  }
}
</script>

<style>
/*
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
*/
@import './assets/css/styles.css'
</style>
