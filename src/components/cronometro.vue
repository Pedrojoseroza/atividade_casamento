<script></script>
<template>
  <section class="cronometro">
    <h2>
      Quanto tempo falta para o grande momento:
    </h2>
    <div>
      <span>
        00:00:00
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
  font-size: 15rem;
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
