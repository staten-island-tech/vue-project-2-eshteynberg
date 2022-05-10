<template>
<body>
  

  <div class="container">
    
      <img src="/project/components/img/placeholder.png" alt="">
      <splash class="test"></splash>
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
  margin-left: -1.5rem;

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

