<template>
  <div class="Post">
    <h3>{{ title }}</h3>
    <h4>{{ desc }}</h4>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Title',
    },
    description: {
      type: String,
      default: 'Description',
    },
  },
}
</script>

<style>
.Post {
  width: 40%;
  display: flex;
  border: solid black;
}
</style>