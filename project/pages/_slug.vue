<template>
  <div>
    <!-- <h1>{{ article.title }}</h1> -->

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
h1{
  text-align: center;
  size: 10rem;
}

.nuxt-content h2 {
    color: aliceblue;
    text-align: center;
}

.nuxt-content img{
  left: 10rem;
  align-content: center;
}

</style>