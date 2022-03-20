<template>
  <div>
    <Blogpost v-for="blog in blogs" :key="blog.number" :post="blog"></Blogpost>
  </div>
</template>

<script>
export default {
  props: {
    blogs: Array,
  },
}
</script>

<style>
</style>