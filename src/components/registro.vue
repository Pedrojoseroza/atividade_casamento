<script></script>

<template>
    <section class="registrar">
    <div>
    <h2>
      Registry
    </h2>
    <p>
      Your presence is the most cheribshed gift. Should you wish to contribute, we’ve created a honeymoon registry to help us to embark on a memorable adventure to the Amalfi Coast
    </p>
    <button>Go to Registry</button>
    </div>
  </section>
</template>
<style scoped>

.registrar {
  background-image: url('/fundo_do_registro.png');
  height: 75vh;
  margin: 0 0 30px 0;
  background-position: contain;

}
.registrar div {
  color: white;
  text-align: center;
}
.registrar div h2 {
  font-size: 5rem;
  padding: 10vh 0 10px 0;
  font-family: 'Aboreto', sans-serif;
}
.registrar div p {
  font-size: 1.8rem;
  margin: 20px 0;
  padding: 0 20vw;
}
.registrar div button {
  border: 0;
  background-color: #3A4D34;
  min-width: 30vw;
  min-height: 10vh;
  border-radius: 40px;
  margin: 40px 0 0 0;
  font-family: 'Aboreto', sans-serif;
  color: white;
  font-size: 2rem;
}
.registrar div button:hover {
    cursor: pointer;
}
@media screen and (max-width: 900px) {
  .registrar {
    height: 50vh;
  }
  .registrar div h2 {
    font-size: 3rem;
  }
  .registrar div p {
    font-size: 1.2rem;
    font-family: sans-serif;
    padding: 0 10vw;
  }
  .registrar div button {
    padding: 0 5vw;
    font-size: 1rem;
    margin: 20px 0 0 0;
  }
  
}
</style>
