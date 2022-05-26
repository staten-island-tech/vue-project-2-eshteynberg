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
          :description="blogpost.description"
          :image="blogpost.image"
          :slug="blogpost.slug"
        ></Post>
       
      </div>
       <quotepg class="quotes"></quotepg>
    </div>
  </body>
</template>


<script>
import photospg from '../components/photospg.vue'
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
</script>

<style>
.container {
  margin: 0 auto;
  padding: 0;
  box-sizing: border-box;
  font-size: 62.5%;
  background-color: #b2966f;
}

/* media queries */

@media (max-width: 200000px) {

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
  width: 10rem;
}

.photos {
  height: 5rem 3rem;
  overflow: hidden;
}
}

@media (max-width: 768px) {

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
}

</style>

