<template>
  <div>
    <h1>Back to <a href="/cuisines">the map</a></h1>
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
  </div>
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
      .where({ tags: { $contains: 'mexican' } })
      .fetch()
  },
}
</script>

<style>
</style>