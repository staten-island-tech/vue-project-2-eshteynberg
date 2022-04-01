<template>
  <div>
    <h1>Satina's Food Blog</h1>
    <div><Post
    v-for= "blogpost in blogposts" :key = "blogpost.title" :title="blogpost.title" :desc="blogpost.description"></Post></div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      blogposts:[],
    }
  },
  head(){
    return{
      title:`Blog`
    }
  },
  async fetch() {
    this.blogposts = await this.$content('blogposts').fetch()
  },


}
</script>
