<template>
  <div class="Post">
    <nuxt-link class="link" :to="{ name: 'slug', params: { slug: slug } }"
      >Link</nuxt-link>
    <h3 class="title">{{ title }}</h3>

    <h4 class="description">{{ desc }}</h4>
  </div>
</template>

<script>
import defaultVue from '../layouts/default.vue'
export default {
  props: {
    title: {
      type: String,
      default: 'Title',
    },
    description: {
      type: String,
      default: 'Description',
    },
    slug: {
      type: String,
      default: '/',
    },
  },
}
</script>

<style>
.Post {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  width: 28rem;
  font-size: 3rem;
  margin: 3.5rem 3rem;
  padding: 2rem;
  align-items: center;
  border-radius: 3rem;
  margin-bottom: 5rem;
  box-shadow: 0 0.25rem 0.5rem 0 rgba(0, 0, 0, 0.2),
    0 0.375rem 1.25rem 0 rgba(0, 0, 0, 0.19);
}

h3 {
  size: 10rem;
}
.image {
  width: 30rem;
}
.link {
  text-decoration: none;
}
</style>