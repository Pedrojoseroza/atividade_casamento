<script setup>

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
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Our Story</a></li>
        <li><a href="#">Details</a></li>
        <li><a href="#">RSVP</a></li>
    </ul>
</section>
</template>

<style scoped>
a{
    color: hsl(0, 0%, 100%);
}
section {
    display: flex;
    height: 15vh;
    width: 100vw;
    align-items: center;
    justify-content: space-between;
    background-color: #A69A9A;
    color: #FFFFFF;
}
section div {
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

section ul{
    display: flex;
    gap: 10px;
    margin: 0 30px 0 0;
}
section ul li a {
    font-family: "Inter", sans-serif;
}

</style>
