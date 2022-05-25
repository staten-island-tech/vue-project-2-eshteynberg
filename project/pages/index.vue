<template>
  <body>
    <div class="container">
      <splash class="test"></splash>
      <featured></featured>
      <div class="all-posts">
        <Post
          class="post"
          v-for="blogpost in blogposts"
          :key="blogpost.description"
          :title="blogpost.title"
          :desc="blogpost.description"
          :img="blogpost.image"
          :slug="blogpost.slug"
        ></Post>
        <quotepg class="quotes"></quotepg>
      </div>
    </div>
  </body>
</template>


<script>
import photospg from '../components/photospg.vue'
import _slugVue from './_slug.vue'
export default {
  components: { photospg },
  name: 'IndexPage',
  data() {
    return {
      blogposts: [],
    }
  },
  head() {
    return {
      title: `Blog`,
    }
  },
  async fetch() {
    this.blogposts = await this.$content('blogposts')
      .sortBy('slug', 'desc')
      .fetch()
  },
}
console.log(this)
</script>

<style>

body{ 
    background-color: #b2966f;
}

.container {
  margin: 0 auto;
  padding: 0;
  box-sizing: border-box;
  font-size: 62.5%;

  margin-left: -2.1rem;
}

.test {
  object-fit: contain;
}

.all-posts {
  flex-wrap: wrap;
  display: flex;
  justify-content: space-evenly;
}
.quotes {
  margin-bottom: 10rem;
}

.photos {
  height: 5rem 3rem;
  overflow: hidden;
}
</style>

