<template>
  <div class="wrapper">
    <!-- <Header /> -->
    <HomeHeader />
    <div class="inner-wrapper">
      <div></div>
      <slot />
    </div>
    <!-- <ColorModePicker /> -->
  </div>
</template>

<script setup>
</script>

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