<template>
  <div>
    <body>
<<<<<<< Updated upstream
      <splash class="test"></splash>
      <div>
        <Post
          v-for="blogpost in blogposts"
          :key="blogpost.title"
          :title="blogpost.title"
          :desc="blogpost.description"
        ></Post>
      </div>
    </body>
=======
    
    <splash class="test"></splash>
    <div><Post class="post"
    v-for= "blogpost in blogposts" :key = "blogpost.title" :title="blogpost.title" :desc="blogpost.description"></Post></div>
     </body>
>>>>>>> Stashed changes
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
<<<<<<< Updated upstream
</style>
=======

.post {
  background-color: #C09165;
  display: flex;
  flex-direction: row ;
  outline-color: black;
  outline: 1rem;


}

</style>

>>>>>>> Stashed changes
