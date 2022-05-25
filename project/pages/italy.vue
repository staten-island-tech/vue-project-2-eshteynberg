<template></template>

<script>
export default {
  async fetch() {
    this.blogposts = await this.$content('blogposts')
      .sortBy({ tags: { $containsAny: ['italy'] } })
      .fetch()
  },
}
</script>

<style>
</style>