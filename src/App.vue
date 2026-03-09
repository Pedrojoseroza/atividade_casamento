<script setup>
import Header from '../src/components/header.vue';
import Banner from './components/banner.vue';
import ListaImagens from './components/listaImagens.vue';
import Registro from './components/registro.vue';
import Cronometro from './components/cronometro.vue';
import Footer from './components/footer.vue';
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
  <section id="registro" >
    <Registro></Registro>
  </section>
  <section id="cronometro">
    <Cronometro></Cronometro>
  </section>
  <footer>
    <Footer></Footer>
  </footer>
</main>
</template>

<style scoped>

header {
  position:sticky;
    top: 0;
    z-index: 2;
}

</style>

