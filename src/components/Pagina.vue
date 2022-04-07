<template>
    <section id="content">
        <h2 class="subheader">Pagina de pruebas</h2>
        <button @click="redirigirAlBlog()">Redirigir</button>
    </section>
</template>

<script>
/* eslint-disable */
export default {
    name:"Pagina",
    methods:{
        redirigirAlBlog(){
            this.$router.push('./blog')
        }
    }
}
</script>