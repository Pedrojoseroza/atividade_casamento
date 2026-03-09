<script>
</script>
<template>
    <section class="banner">
    <h2>
      Jenny & Jason
    </h2>

    <div>
      <p>
With love and grattitude, we invite you to share the enjoy of our wedding day.
Saturday, September 20, 2025
The golden Elm Manor,
St. Augustine New York
      </p>
    </div>
  </section>

</template>

<style scoped>

.banner {
  max-width: 100vw;
}
.banner h2  {
  text-align: center;
  font-size: 10rem;
  font-family: 'Aboreto', sans-serif;
  padding: 20px 0;
}
.banner div {
  background-image: url('/back_image.png');
  min-height: 80vh;
  display: flex;
  align-items: center;
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}
.banner div p {
  font-family: sans-serif;
  font-size: 2.5rem;
  text-align: center;
  padding: 0 20vw;
  color: white;
}
@media screen and (max-width: 900px) {
  .banner h2 {
    font-size: 1.5rem;
    padding: 10px 0;
  }
  .banner div {
    min-height: 30vh;
  }
  .banner div p {
    font-size: 1rem;
    padding: 0 10vw;
  }
}
</style>
