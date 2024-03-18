<template>
  <nav class="scrim-bg site-nav" aria-label="Main Menu">
    <ul class="flex">
      <li class="flex-1">
        <nuxt-link class="btn block" to="/">Home</nuxt-link>
      </li>
      <li class="flex-1">
        <nuxt-link class="btn block" to="/projects">Projects</nuxt-link>
      </li>
    </ul>
  </nav>
</template>

<script setup>
// export default {
//   name: 'Header'
// }
</script>

<style>
.site-nav ul {
  /* display: flex; */
  flex-direction: column;
  max-width: 100%;
  align-items: center;
  width: 70%;
  margin: 0 auto;
}

.site-nav ul li {
  margin-top: 0.5em;
  width: 100%;
}

.site-nav ul li a {
  /* border-color: var(--color-gray-900); */
  background-color: #c3cbdc;
  border-radius: 0;
  color: #171d1e;
  position: relative;
  display: flex;
  justify-content: center;
}

/* .site-nav ul li a::after {
  content: "";
  position: absolute;
  height: 1px;
  width: 5rem;
  background-color: white;
} */

</style>
