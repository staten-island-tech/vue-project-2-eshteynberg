<template>
  <div>
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
.nuxt-content {
  display: grid;
}

.nuxt-content h2 {
  margin-top: 3rem;
  margin-bottom: 2rem;
  align-content: center;
  grid-template-columns: 1fr;
  text-align: center;
  font-family: raleway;
  font-size: 3.5rem;
}
.nuxt-content p {
  text-align: center;
  font-size: 2rem;
  padding: 3rem;
}
.nuxt-content img {
  display: flex;
  margin-left: auto;
  margin-right: auto;
  margin-top: 5rem;
  width: 39rem;
  border: solid black;
  border-radius: 2rem;
}
</style>