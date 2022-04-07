<template>
  <section id="content">
    <h2 class="subheader">Peliculas</h2>

    <!--Listado articulos-->
    <div id="articles">
      <!-- v-for="pelicula in peliculas" v-bind:key="pelicula.title" -->
      <div v-for="pelicula2 in peliculas" v-bind:key="pelicula2.title">
          <PeliculaComponent :pelicula="pelicula2"></PeliculaComponent>
      </div>
    </div>
  </section>
</template>

<script>
/* eslint-disable */
import PeliculaComponent from './PeliculaComponent.vue'
export default {
  name: "Peliculas",
  components:{
      PeliculaComponent
  },
  data(){
      return{
          peliculas:[
              {title:'Batman vs Superman', year:2017, image:"https://www.cinematographe.it/wp-content/uploads/2017/08/justice-league-batman-v-superman.jpg"},
              {title:'Ironman', year:2008, image:"https://www.ultimarazzia.it/wp-content/uploads/2019/09/Iron-man-1280x720.jpg"},
              {title:'El Origen', year:2010, image:"https://www.explicacion.net/wp-content/uploads/2018/08/el-origen.jpg"}
          ]
      }
  }
};
</script>

<style>
</style>