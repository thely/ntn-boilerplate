<template>
  <div class="wrapper">
    <!-- <Header /> -->
    <HomeHeader />
    <div class="inner-wrapper">
      <div></div>
      <nuxt />
    </div>
    <ColorModePicker />
  </div>
</template>

<style>
.wrapper {
  padding-top: 2rem;
}

.inner-wrapper {
  position: relative;
  display: grid;
  grid-template-columns: 1fr 3fr;
  width: 100%;
}
</style>