<template>
  <div class="home-block">
    <div class="home-inner">
      <!-- <Header /> -->
      <img :src="image" />
    </div>

    <div class="left-side">
      <h1>
        <span class="letter">V</span>
        <hr />
        <span class="title">the Sound Girl</span>
      </h1>
      <Header />
    </div>
  </div>
</template>

<script setup>
// import { ref } from 'vue';
const image = "/img/new_homepage.jpg";

</script>

<style>

.home-block {
  position: relative;
  display: grid;
  grid-template-columns: 1fr 3fr;
  width: 100%;
}

.home-block .home-inner {
  order: 1;
}

.home-block img {
  display: block;
  max-width: 100%;
  border: 1px solid white;
  border-left: 2em solid white;
}

.home-block h1 {
  line-height: 1;
  text-align: center;
  /* display: flex; */
  /* flex-direction: column; */
  /* margin-top: -5rem; */
  display: grid;
  grid-template-rows: 1fr 1px 1fr;
  align-items: center;
  justify-items: center;

  padding: 0.5rem 1.75rem;

  justify-content: space-around;
  background-image: url(/img/new_homepage.jpg);
  background-size: 500%;
  background-position: right;
  border: 1px solid white;
  margin-top: -2rem;
  margin-bottom: 1.4rem;
  
  position: relative;
}

.home-block h1::after {
  content: "";
  display: block;
  position: absolute;
  bottom: -70vh;
  height: 80vh;
  width: 40px;
  background-color: rgba(32, 32, 32, 0.5);
  border-radius: 30px;
  z-index: -1;
  border: 10px solid #4645455c;
  box-shadow: 0 0 0 10px rgba(60, 58, 58, 0.9);
}

.home-block h1 .letter {
  font-size: 13rem;
  /* border-bottom: 0.1rem dashed var(--highlight-color); */
  /* margin-bottom: 0.65rem; */
  line-height: 0.8;
  /* padding-bottom: 1.4rem; */
}

.home-block hr {
  border-top: 2px dashed white;
  width: 70%;
}

.home-block h1 .title {
  font-size: 3rem;
}
</style>