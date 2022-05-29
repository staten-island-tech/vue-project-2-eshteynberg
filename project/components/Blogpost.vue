<template>
  <div>
    <img :src="post.img" />
    <h1>{{ post.title }}</h1>
    <h2>{{ post.desc }}</h2>
    <h3>{{ post.location }}</h3>
    <h4>{{ post.cuisine }}</h4>
  </div>
</template>

<script>
export default {
  props: {
    post: Object,
  },
}
</script>

<style>

</style>