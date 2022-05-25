<template>
  <body>
    <div class="all-posts">
      <Post></Post>
    </div>
  </body>
</template>

<script>
export default {
  data() {
    return {
      blogposts: [],
    }
  },
  async fetch() {
    this.blogposts = await this.$content('blogposts')
      .where({ tags: 'italian' })
      .fetch()
  },
}
</script>

<style>
</style>