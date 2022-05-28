<template>
  <div>
    <div class="title">
      <h1>ITALIAN CUISINE</h1>
    </div>

    <div>
      <h1>Back to <a class="return" href="/cuisines">the map</a></h1>
    </div>

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
      .where({ tags: { $contains: 'italian' } })
      .fetch()
  },
}
</script>

<style>
.return {
  text-decoration: none;
  color: black;
}

.title {
  margin-top: 1.5rem;
  align-content: center;
  padding: 3rem;

  display: grid;
  grid-template-columns: 1fr;
  text-align: center;
  margin: auto;
  font-family: raleway;
  font-size: 2rem;
  box-shadow: 0px 0px 40px 20px rgba(0, 0, 0, 0.05);
}

.all-posts {
  flex-direction: row;
  display: flex;
}
</style>