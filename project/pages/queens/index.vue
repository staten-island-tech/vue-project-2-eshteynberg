<template>
  <div>
    <Head></Head>
    <Blogpost
      v-for="post in filterBlog()"
      :key="post.number"
      :post="post"
    ></Blogpost>
  </div>
</template>

<script>
export default {
  data() {
    return {
      blogs: [
        {
          number: 1,
          title: 'best sushi spots',
          cuisine: 'Japanese',
          desc: 'ddneefewf',
          text: 'rggfhggjjgj',
          location: 'Brooklyn',
          img: 'https://images.unsplash.com/photo-1562436260-8c9216eeb703?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTl8fHN1c2hpfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60',
        },
        {
          number: 2,
          title: 'best dumplings',
          cuisine: 'Chinese',
          desc: 'fefefegf',
          location: 'Brooklyn',
          text: 'rggfhggjjgj',
          img: 'https://images.unsplash.com/photo-1496116218417-1a781b1c416c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8N3x8Y2hpbmVzZSUyMGR1bXBsaW5nc3xlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60',
        },
        {
          number: 3,
          title: 'best kebab',
          cuisine: 'Middle Eastern',
          desc: 'rgrgrg',
          text: 'rggfhggjjgj',
          location: 'Manhattan',
          img: 'https://images.unsplash.com/photo-1595777216528-071e0127ccbf?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8OXx8a2ViYWJ8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60',
        },
        {
          number: 4,
          title: 'my favorite ramen',
          cuisine: 'Japanese',
          desc: 'eregregt',
          text: 'rggfhggjjgj',
          location: 'Queens',
          img: 'https://images.unsplash.com/photo-1591814468924-caf88d1232e1?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8M3x8cmFtZW58ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60',
        },
        {
          number: 5,
          title: 'my favorite roasted duck',
          cuisine: 'Chinese',
          desc: 'fefggrg',
          text: 'rggfhggjjgj',
          location: 'Queens',
          img: 'https://static01.nyt.com/images/2019/01/28/dining/kc-peking-duck/kc-peking-duck-articleLarge-v2.jpg',
        },
        {
          number: 6,
          title: 'best mochi',
          cuisine: 'Japanese',
          desc: 'ssfdfsf',
          text: 'rggfhggjjgj',
          location: 'Manhattan',
          img: 'https://images.ctfassets.net/3s5io6mnxfqz/7bBkcNBvM87q4raaLMIovp/f0c7706c4810697c94699510b1d705b7/AdobeStock_399889639.jpeg?fm=jpg&w=900&fl=progressive',
        },
        {
          number: 7,
          title: 'best falafel spots',
          cuisine: 'Middle Eastern',
          desc: 'grgukuk',
          text: 'rggfhggjjgj',
          location: 'Brooklyn',
          img: 'https://images.unsplash.com/photo-1547058881-aa0edd92aab3?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1470&q=80',
        },
        {
          number: 8,
          title: 'best turkish desserts',
          cuisine: 'Middle Eastern',
          desc: 'ykjyotutoy',
          text: 'rggfhggjjgj',
          location: 'Brooklyn',
          img: 'https://images.unsplash.com/photo-1598110750624-207050c4f28c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8N3x8dHVya2lzaCUyMGRlc3NlcnRzfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60',
        },
        {
          number: 9,
          title: 'best chinese desserts',
          cuisine: 'Chinese',
          desc: 'ykjyotutoy',
          text: 'rggfhggjjgj',
          location: 'Manhattan',
          img: 'https://images.unsplash.com/photo-1630859311469-289b6a574bdc?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTN8fGNoaW5lc2UlMjBkZXNzZXJ0c3xlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60',
        },
      ],
    }
  },
  methods: {
    filterBlog() {
      return this.blogs.filter((b) => b.location === 'Queens')
    },
  },
}
</script>

<style>
</style>