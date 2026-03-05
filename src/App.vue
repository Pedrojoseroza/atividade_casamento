<script setup>
import Header from '../src/components/header.vue';
import Banner from './components/banner.vue';
import ListaImagens from './components/listaImagens.vue';
import listaImagens from './components/listaImagens.vue';
</script>

<template>
<header>
  <Header></Header>
</header>
<main>
  <section id="banner">
    <Banner></Banner>
  </section>
  <section id="grid_de_imagens">
    <ListaImagens></ListaImagens>
  </section>
</main>
</template>

<style scoped>
</style>
