<template>
  <div class="container">
    <body>
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
        ></Post>
        <quotepg class="quotes"></quotepg>
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
  background-color: #B2966F;
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

