<script setup>
import { ref } from 'vue';
const tempo = ref(1000000);
const segundos = ref(60);
const minutos = ref(tempo.value % 60);
const horas = ref(Math.round(tempo.value / (60 * 60)));
if (tempo.value > 0) {
  const cronometroSeg = setInterval(() => {
    segundos.value--
    tempo.value--;
  }, 1000);
  const cronometroMin = setInterval(()=> {
    segundos.value = 60;
    minutos.value--
  }, 60000)
  const cronometroHora = setInterval(() => {
    minutos.value = 60;
    horas.value--;
  }, 360000);
}
</script>
<template>
  <section class="cronometro">
    <h2>
      Quanto tempo falta para o grande momento:
    </h2>
    <div>
      <span>
        {{ horas }}:
        {{ minutos }}:
       {{ segundos }}
      </span>
    </div>
  </section>
</template>
<style scoped>

.cronometro {
  padding: 5vh 10vw;
}
.cronometro h2 {
  text-align: center;
  font-size: 3rem;
  font-family: 'Aboreto', sans-serif;
  margin: 0 0 20px 0;
}
.cronometro div {
  display: flex;
  justify-content: center;
}
.cronometro div span{
  width: 65vw;
  background-color: #D9D9D9;
  text-align: center;
  font-size: 10rem;
  border-radius: 20px;
}
@media screen and (max-width: 900px) {
  .cronometro h2 {
    font-size: 2rem;
  }
  .cronometro div span {
    font-size: 4.5rem;
  }
}
</style>
