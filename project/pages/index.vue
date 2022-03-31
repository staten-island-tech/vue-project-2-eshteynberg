<template>
  <div>
    <h1>Satina's Food Blog</h1>
    <div>v-for= "blogpost in blogposts" :key = "blogpost.title"</div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      title: `Blog`,
    }
  },
  async fetch() {
    this.blogposts = await this.$content('blogposts').fetch()
  },
}
</script>
