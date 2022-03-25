<template>
  <div>
    <Head></Head>
    <Blogpost
      v-for="post in filterBlog()"
      :key="post.number"
      :post="post"
    ></Blogpost>
  </div>
</template>

<script>
export default {
  methods: {
    filterBlog() {
      return this.getBlogs().filter((b) => b.location === 'Manhattan')
    },
    getBlogs() {
      return this.$blogs
    },
  },
}
</script>

<style>
</style>