<template>
  <div class="Post">
    <h3 class="title">{{ title }}</h3>

    <img class="image" src="{{" image }} alt="" />

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
  width: 26%;
  height: 20rem;
  margin: 1rem auto;
  align-items: center;
  border-radius: 3rem;
  margin-bottom: 5rem;
  font-size: 2rem;
}
</style>