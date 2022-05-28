<template>

  <div class="Post">
    
    <nuxt-link class="link" :to="{ name: 'slug', params: { slug: slug } }">{{
      title
    }}</nuxt-link>
    <nuxt-link :to="{ name: 'slug', params: { slug: slug } }">
      <img class="image-post" :src="image" alt="test" />
    </nuxt-link>

    <p class="post-description">{{ description }}</p>
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
      default: 'description',
    },
    body: {
      type: String,
      default: 'body',
    },
    slug: {
      type: String,
      default: '/',
    },
    image: {
      type: String,
    },
  },
}
</script>

<style>
.link {
  text-decoration: none;
  text-align: center;
}

.Post:hover {
  background-color: tomato;
  transform: scale(1.1);
}

.image-post:hover {
  transform: scale(1.1);
}

/* media queries */

@media (max-width: 20000px) {
  .Post {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    width: 28rem;
    font-size: 2rem;
    margin: 3.5rem 3rem;
    padding: 2rem;
    align-items: center;
    border-radius: 3rem;
    margin-bottom: 5rem;
    box-shadow: 0 0.25rem 0.5rem 0 rgba(0, 0, 0, 0.2),
      0 0.375rem 1.25rem 0 rgba(0, 0, 0, 0.19);
      background-color: turquoise;
  }

  .post-description {
    text-align: center;
  }
  .image-post {
    width: 25rem;
    border-radius: 1rem;
    border: solid black;
    transition: 300ms;
  }
  .link {
    text-decoration: underline;
    color: black;
    padding: 3rem;
  }

}

@media (max-width: 768px) {
  .Post {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    width: 14rem;
    font-size: 2rem;
    padding: 2rem;
    align-items: center;
    border-radius: 3rem;
    box-shadow: 0 0.25rem 0.5rem 0 rgba(0, 0, 0, 0.2),
      0 0.375rem 1.25rem 0 rgba(0, 0, 0, 0.19);
  }

  .post-description {
    text-align: center;
  }
  .image-post {
    width: 15rem;
    border-radius: 1rem;
  }
}

@media (max-width: 414px) {
  .Post {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    width: 14rem;
    font-size: 2rem;
    padding: 2rem;
    align-items: center;
    border-radius: 3rem;
    box-shadow: 0 0.25rem 0.5rem 0 rgba(0, 0, 0, 0.2),
      0 0.375rem 1.25rem 0 rgba(0, 0, 0, 0.19);
  }

  .post-description {
    text-align: center;
  }
  .image-post {
    width: 10rem;
    border-radius: 1rem;
  }
}
</style>