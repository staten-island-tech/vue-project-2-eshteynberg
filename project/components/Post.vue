<template>
  <div class="Post">
    <img class="image-post" :src="image" alt="test" />
    <nuxt-link class="link" :to="{ name: 'slug', params: { slug: slug } }">{{
      title
    }}</nuxt-link>

    <p class="post-description">{{ description }}</p>
    
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
      default: 'description',
    },
    body: {
      type: String,
      default: 'body',
    },
    slug: {
      type: String,
      default: '/',
    },
    image: {
      type: String,
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

.post-description {
  size: 0.5rem;
  text-align: center;

}
.image-post {
  width: 25rem;
  border-radius: 1rem;

}
.link {
  text-decoration: none;
}
</style>