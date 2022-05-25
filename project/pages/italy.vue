<template>
  <body>
    <div class="all-posts">
      <Post
        class="post"
        v-for="blogpost in blogposts"
        :key="blogpost.description"
        :title="blogpost.title"
        :description="blogpost.description"
        :image="blogpost.image"
        :slug="blogpost.slug"
      >
      </Post>
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
      .where({ tags: { $contains: 'italian' } })
      .fetch()
  },
}
</script>

<style>
</style>