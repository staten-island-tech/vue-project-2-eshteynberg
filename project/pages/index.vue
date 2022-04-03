<template>
  <div>
    <Head></Head>
    <Featured :blogs="blogs"></Featured>
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
</style>
