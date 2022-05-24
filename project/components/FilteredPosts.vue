<template>
  <body>
    <div class="filtered-posts">
      <h1>Recent Posts</h1>
      <div class="Parent">
      
          <img class="img" src="./img/meat-lasagna-1200.jpg" alt="" />
      <img class="img" src="./img/spaghetti-squash-soup.jpg" alt="" />
        </div>
    </div>
  </body>
</template>

<script>
export default {}
</script>

<style scoped>
.h1 {
  justify-content: center;
  margin-top: 2rem;
}
.filtered-posts {
  background-color: #c09165;
  padding: 20rem;
  width: 5rem;
  margin-left: 25rem;
}
.img {
  width: 20rem;
  padding: 2rem;
  margin: 3rem;
}
.parent {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(4, 1fr);
  grid-column-gap: 0px;
  grid-row-gap: 0px;
}
</style>