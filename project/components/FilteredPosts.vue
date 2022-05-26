<template>
  <body>
    <div class="container">
      <!-- <div class="title">
      <h1>Recent Posts</h1>
</div> -->
 
<section class="ameri">
        <div class="child1">
        <img class="img" src="../static/img/ameri1.jpg" alt="" />
       
        </div>
        <div class="child2">
        <img class="img" src="../static/img/ameri2.jpg" alt="" />
</div>
<div class="child3">
        <img class="img" src="../static/img/ameri3.jpg" alt="" />
        </div>
        <div class="child4">
        <img class="img" src="../static/img/ameri4.jpg" alt="" />
</div>
<div class="child5">
        <img class="img" src="../static/img/ameri5.jpg" alt="" />
        </div>

</section>

<section class="mediterannean">
        <div class="child6">
        <img class="img" src="../static/img/med1.jpg" alt="" />
</div>
<div class="child7">
        <img class="img" src="../static/img/med2.jpg" alt="" />
</div>
<div class="child8">
        <img class="img" src="../static/img/med3.jpg" alt="" />
</div>
<div class="child9">
        <img class="img" src="../static/img/med4.jpg" alt="" />
</div>
</section>
      </div>

  </body>
</template>

<script>
export default {}
</script>

<style scoped>
/* .title{
font-family: Raleway;
font-size: 1.5rem;

} */
.container {
  background-color: #c09165;
  padding: 10rem;
  width: 48rem;
margin: auto;
margin-top: 5rem;
display: grid;
gap: 3rem;
grid-template-columns: repeat(3,1fr);
justify-content: center;
align-content: space-between;
}

.child1{
  grid-column: span 2;
}
.img {
  width: 20rem;
  height: 60%;
  padding: 2rem;
  box-shadow: 0px 0px 40px 20px rgba(0, 0, 0, 0.05);

}




</style>