<template>
  <div>
    <div class="title">
      <h1>MEXICAN CUISINE</h1>
    </div>

    <div class="return">
      <h1>Back to <a href="/cuisines">the map</a></h1>
    </div>

    <div class="all-posts">
      <Post
        class="post"
        v-for="blogpost in blogposts"
        :key="blogpost.description"
        :title="blogpost.title"
        :description="blogpost.description"
        :image="blogpost.image"
        :alt="blogpost.alt"
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
.light {
  background-color: var(--light-bg);
  color: var(--light-font);
}

.dark {
  background-color: var(--dark-bg);
  color: var(--dark-font);
}

.return {
  padding: 1.5rem;
  border-radius: 3rem;
  display: flex;
  align-content: flex-start;
  width: 15rem;
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