<script setup>
</script>

<template>
    <div>
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
    </div>
</template>
<style scoped>

ul {
  display: grid;
  grid-template-columns: 1fr 1fr;
   place-items: center;
  gap: 15px;
  margin: 30px 0;
  align-self: center;
  padding: 0 20vw;
}
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
}
ul li:hover {
  transition: height, 0.5s;
  transition: width, 0.5s;
  width: 26vw;
  height: 81vh;
}
ul li#story {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/public/imagem_anel_1.png');
}

ul li#details {
  background-image:linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/public/imagem_mesa_com_pera_1.png');
}
ul li#respond {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/public/imagem_igreja_1.png');
}
ul li#registry {
  background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/public/imagem_rosa_seca_1.png');
}
ul li p {
  text-align: center;
  color: white;
  text-decoration: underline;
  font-size: 2.4rem;
}

</style>