<template>
<div>
  <img class="coffee" src="./img/coffee.png" alt="" />
   <div class="NavBar">

    
    <a class="btn" href="/">Home</a>
    <a class="btn" href="/about">About</a>
    <a class="btn" href="/cuisines">Cuisines</a>
    <a class="btn" href="/contact">Contact Us</a>
  </div>
  </div>
 
</template>

<style scoped>
.NavBar {
  background-color: #b2966f;
  height: 6rem;
  text-decoration: none;
  display: flex;
  align-items: center;
}

.coffee {
  z-index: -1;
  margin-left: 4rem;
}

.btn {
  display: inline-block;
  background-color: #b2966f;
  color: white;
  flex-flow: row;
  justify-content: space-between;
  margin-bottom: 1rem;
  margin-left: 18rem;
  border: #b2966f solid;
  font-size: 1.25rem;
  text-align: center;
}
</style>

<script>
export default {
  navbar: Object,
}
</script>
