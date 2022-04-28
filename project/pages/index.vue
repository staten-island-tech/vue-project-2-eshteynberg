<template>
  <div class="container">
    <body>
      <splash class="test"></splash>
      <h1>
        pls ignore ugly borders just wanted a guide to where the things stop
      </h1>
      <div class="all-posts">
        <Post
          class="post"
          v-for="blogpost in blogposts"
          :key="blogpost.title"
          :title="blogpost.title"
          :desc="blogpost.description"
          :img="blogpost.image"
        ></Post>
        <quotepg class="quotes"></quotepg>
        <photospg class="photos"></photospg>
      </div>
    </body>
  </div>
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
    this.blogposts = await this.$content('blogposts').fetch()
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
  width: 10rem;
  overflow: hidden;
}

</style>

