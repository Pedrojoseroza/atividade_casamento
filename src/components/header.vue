<script setup>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
  function mostrarlista () {
    const bg = document.querySelector('section nav div');
    bg.classList.toggle('ativo');
  }
</script>
<template>
<section>
    <div>
        <h1>
            <a href="../App.vue">J & J</a>
        </h1>
        <p>
            June, 23rd, 2026
        </p>
    </div>
    <nav>
      <div @click="mostrarlista">
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Our Story</a></li>
          <li><a href="#">Details</a></li>
          <li><a href="#">RSVP</a></li>
        </ul>
      </div>
        <span class="toggle" @click="mostrarlista">
          <font-awesome-icon icon="fa-solid fa-bars" />
        </span>
    </nav>
</section>
</template>

<style scoped>
a{
    color: hsl(0, 0%, 100%);
}
section {
    display: flex;
    height: 15vh;
    align-items: center;
    justify-content: space-between;
    background-color: #a69a9ab6;
    color: #FFFFFF;
    position:sticky;
    top: 0;
    z-index: 2;
}
section > div {
    padding: 0 0 0 20px;
    display: flex;
    align-items: center;
    margin: 0 0 0 30px;
    font-family: "Jacques Francois", serif;
}
section div h1 {
    margin: 0 20px 0 0;
}
section div h1 a {
    text-decoration: none;
}
section nav {
  margin: 0 20px 0 0;
}
section nav ul {
    display: flex;
    gap: 10px;
    padding: 0 10px 0 0;
}
section nav span {
  display: none;
}
section nav ul li a {
    font-family: "Inter", sans-serif;
    text-decoration: none;
}
section nav ul li a:hover {
  text-decoration: underline;
}
@media screen and (max-width: 900px) {
  section {
    height: 10vh;
    justify-content: space-between;
  }
  section > div {
    padding: 0 0 0 0px;
 }
 section div h1 {
  font-size: 2rem;
}

 section div p {
  display: none;
 }
 section nav div {
   display: none; /* Oculto por padrão */
  position: fixed;
  z-index: 1;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0,0,0,0.5); /* Fundo semi-transparente */
 }
 section nav span{
  display: block;
  margin: 0 20px 0 0;
  font-size: 2rem;
 }
 section nav div.ativo {
  display: block;
 }
 section nav div.ativo ul {
  display: block;
  margin: 20vh 20vw;
  border-radius: 10px;
  background-color: #394826;
 }
 section nav div.ativo ul li {
  margin: 10px 0;
  font-size: 4rem;
  text-align: center;
 }
}
</style>
