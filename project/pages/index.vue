<template>
  <div>
    <body>
    <NavBar></NavBar>
    <splash class="test"></splash>
    <div><Post
    v-for= "blogpost in blogposts" :key = "blogpost.title" :title="blogpost.title" :desc="blogpost.description"></Post></div>
     </body>
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

<style>

.body{
  background-color: #B2966F;
}

.test{
  object-fit: contain;
}
</style>