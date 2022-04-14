<template>

<body>
  <div class="filtered-posts">
<h1>Recent Posts</h1>
<div class="Parent">
  <div class="div1">
    <img src="./img/meat-lasagna-1200.jpg" alt="">
  </div>
<div class="div2">
  <img src="./img/spaghetti-squash-soup.jpg" alt="">
</div>
  </div>
  </div>
</body>
  
</template>

<script>
export default {

}
</script>

<style>


img{
  size: 50%;
  object-fit: contain;
}
.h1{
  justify-content: center;
  margin-top: 2rem;
}
.filtered-posts{
  background-color: #C09165;
  padding: 20rem;
  max-width: 10rem;
  margin-left: 25rem;
}
.parent {
display: grid;
grid-template-columns: 1.5fr 0.8fr 1fr;
grid-template-rows: 1.5fr 1fr 1.3fr;
grid-column-gap: 15px;
grid-row-gap: 0px;
 width: 100%;
  height: 100%;
}

.div1 { grid-area: 1 / 1 / 2 / 2; object-fit: contain;  }
.div2 { grid-area: 1 / 2 / 2 / 3; }
.div3 { grid-area: 1 / 3 / 2 / 4; }
.div4 { grid-area: 2 / 1 / 3 / 2; }
.div5 { grid-area: 2 / 2 / 3 / 3; }
.div6 { grid-area: 2 / 3 / 3 / 4; }
.div7 { grid-area: 3 / 1 / 4 / 2; }
.div8 { grid-area: 3 / 2 / 4 / 3; }
.div9 { grid-area: 3 / 3 / 4 / 4; }
</style>