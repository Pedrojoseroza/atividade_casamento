<script setup>
</script>

<template>
    <section>
        <ul>
      <li id="story">
        <p>Our Story</p>
      </li>
      <li id="details">
        <p>Details</p>
      </li>
      <li id="respond">
        <p>RSVP</p>
      </li>
      <li id="registry">
        <p>Registry</p>
      </li>
    </ul>
    </section>
</template>
<style scoped>
section
ul {
  display: grid;
  grid-template-columns: 1fr 1fr;
   place-items: center;
  gap: 15px;
  margin: 30px 0;
  align-self: center;
  padding: 0 20vw;
}section
ul li {
  width: 25vw;
  height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  border-radius: 10px;
  font-family:'Aboreto', sans-serif ;
}section
ul li:hover {
  transition: height, 0.5s;
  transition: width, 0.5s;
  width: 26vw;
  height: 81vh;
}section
ul li#story {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/public/imagem_anel_1.png');
}
section
ul li#details {
  background-image:linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/public/imagem_mesa_com_pera_1.png');
}section
ul li#respond {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/public/imagem_igreja_1.png');
}section
ul li#registry {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/public/imagem_rosa_seca_1.png');
}section
ul li p {
  text-align: center;
  color: white;
  text-decoration: underline;
  font-size: 2.4rem;
}
@media screen and (max-width: 900px) {
  section ul {
    display: block;
    padding: 0 30px;
   }
  section ul li {
    height: 40vh;
    width: 50vw;
    margin: 10px 0;
  }
   section ul li:hover {
     height: 42vh;
     width: 52vw;
  }
  section ul li p {
    font-size: 1.5rem;
  }
}
</style>
