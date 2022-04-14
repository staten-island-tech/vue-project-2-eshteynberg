<template>
  <div>
    <body>
      <splash class="test"></splash>
       <h1>pls ignore ugly borders just wanted a guide to where the things stop</h1>
      <div class="all-posts">
      
        <Post class="post"
          v-for="blogpost in blogposts"
          :key="blogpost.title"
          :title="blogpost.title"
          :desc="blogpost.description"
          :img="blogpost.image"
        ></Post>
      </div>
    </body>
  </div>
</template>


<script>
export default {
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
body {
  background-color: #b2966f;
}

.test {
  object-fit: contain;
}



.all-posts{

  display: grid;
grid-template-columns: repeat(3, 1fr);
grid-template-rows: repeat(5, 1fr);
grid-column-gap: 0px;
grid-row-gap: 0px;
justify-content: center;
}
</style>

