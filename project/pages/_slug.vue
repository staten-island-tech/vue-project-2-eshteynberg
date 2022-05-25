<template>
  <div>
    <h1>{{ article.title }}</h1>

    <nuxt-content :document="article" />
  </div>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const article = await $content('blogposts', params.slug).fetch()
    console.log(article)
    return { article }
  },
}
</script>

<style>
</style>