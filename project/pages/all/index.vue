<template>
  <div>
    <Head></Head>
    <Blogpost
      v-for="post in getBlogs()"
      :key="post.number"
      :post="post"
    ></Blogpost>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  methods: {
    getBlogs() {
      return this.$blogs
    },
  },
}
</script>
