<template>
<<<<<<< Updated upstream
  <div class="Post">
    <h3>{{ title }}</h3>
    <h4>{{ desc }}</h4>
  </div>
=======
    <div class="Post">
        <h3 class="title">{{ title }}</h3>

<img class="image-blog" src= {{  }} alt="">

        <h4 class="description">{{ desc }}</h4>
    </div>
>>>>>>> Stashed changes
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
<<<<<<< Updated upstream
.Post {
  width: 40%;
  display: flex;
  border: solid black;
=======
.Post { 
    width: 40%;
    display: flex;
    border-style: solid;
    border: solid #000 1rem;
>>>>>>> Stashed changes
}
</style>