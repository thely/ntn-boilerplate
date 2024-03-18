
<template>
  <main>
    <section class="self-center flex flex-col flex-1 items-center justify-center">
      <h1 class="title text-center">{{ HOME.title }}</h1>
      <ContentRendererMarkdown :value="result" v-if="result" />
    </section>

    <section class="self-center flex">
      <p>
        {{ HOME.contacttext }}
        <a href="/contact">{{ HOME.contactbtntext }}</a>
      </p>
    </section>

    <section class="mt-8">
      <!-- {{ HOME }} -->
      <h3 class="text-primary-600 dark:text-primary-400 max-w-5xl mx-auto">Latest blog post</h3>
      <PostList post-type="blog" :amount="1" />
    </section>
  </main>
</template>

<script setup>
import { onMounted } from 'vue'
import HOME from '../content/site/home.json'
import markdownParser from '@nuxt/content/transformers/markdown'

// import { parseMarkdown } from '~/utils/parseMarkdown'
useState('headerImage', () => '')
// hea
const headerImage = useState('headerImage')
// console.log(headerImage);
const text = HOME.abouttext

// const result = ref(null)
// const loadMarkdown = async () => {
//   const data = await $fetch('https://example.com/page.md')
//   result.value = await parseMarkdown(data)
// }
// loadMarkdown()
const result = ref(null)

onMounted(async () => {
  console.log(HOME)
  headerImage.value = HOME.headerimg
  result.value = await markdownParser.parse('custom.md', text)
  console.log(result.value);
  console.log(headerImage);
})
</script>