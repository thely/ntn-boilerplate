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
  display: flex;
  align-items: center;
  flex-direction: column;
  list-style-type: none;
  max-width: 100%;
  margin: 0 auto;
  padding-left: 0;
  width: 70%;
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
  display: flex;
  justify-content: center;
  padding: 0.7em;
  position: relative;
  text-decoration: none;
}

/* .site-nav ul li a::after {
  content: "";
  position: absolute;
  height: 1px;
  width: 5rem;
  background-color: white;
} */

</style>
