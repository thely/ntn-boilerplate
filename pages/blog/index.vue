<template>
  <main>
    <section v-if="posts" class="w-full max-w-5xl mx-auto">
      <h1 class="title">Blogaa</h1>
      <PostList post-type="blog" :amount="10" />
    </section>
  </main>
</template>

<script setup>
const { posts } = await useAsyncData('posts', 
  () => queryContent('blog').find()
)
</script>
