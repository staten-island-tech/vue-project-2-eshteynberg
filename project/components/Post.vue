<template>
    <div class="Post">
        <h3 class="title">{{ title }}</h3>

<img class="image" src= {{ image }} alt="">

        <h4 class="description">{{ desc }}</h4>
    </div>
</template>

<script>
import defaultVue from '../layouts/default.vue'
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
    slug: {
        type: String,
        default: '/',
    },
  },
}
</script>

<style>
.Post { 
    width: 10rem;
    display: flex;
    border-style: solid;
    border: solid #000 1rem;
     background-color: #C09165;
  flex-direction: row ;
  outline-color: black;
  outline: 1rem;
  flex-wrap: wrap;
  display: flex;
  justify-content: center;
}

</style>