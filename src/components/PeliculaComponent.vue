<template>
  <article class="article-item">
    <div class="image-wrap">
      <img
        :src="pelicula.image"
        :alt="pelicula.title"
        :title="pelicula.title"
      />
    </div>

    <h2>{{ pelicula.title }}</h2>
    <span class="date"> {{ pelicula.year }} </span>
    <a href="#">Leer más</a>

    <div class="clearfix"></div>
  </article>
</template>

<script>
export default {
  name: "PeliculaComponent",
  props:['pelicula']
};
</script>

<style>
</style>