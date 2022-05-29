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

.light{
  background-color: var(--light-bg);
  color: var(--light-font);
}

.dark{
  background-color: var(--dark-bg);
  color: var(--dark-font)
}

@media (max-width: 200000px) {
.nuxt-content h2 {
  margin-top: 3rem;
  margin-bottom: 2rem;
  align-content: center;
  grid-template-columns: 1fr;
  text-align: center;
  font-family: raleway;
  font-size: 3.5rem;
  box-shadow: 0px 0px 40px 20px rgba(0, 0, 0, 0.05);
  
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
  border-radius: 2rem;
}
}
@media (max-width: 786px) {
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
  width: 20rem;
  border-radius: 2rem;
}
}
@media (max-width: 414px) {
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
  width: 15rem;
  border-radius: 2rem;
}
}

</style>