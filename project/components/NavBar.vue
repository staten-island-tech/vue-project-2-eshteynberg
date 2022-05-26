<template>
  <div class="NavBar">
    <img class="coffee" src="/img/coffee.png" alt="" />
    <a class="btn" href="/">Home</a>
    <a class="btn" href="/about">About</a>
    <a class="btn" href="/cuisines">Cuisines</a>
    <a class="btn" href="/contact">Contact Us</a>
  </div>
</template>

<style scoped>

.btn:hover {
  transform: translateY(-0.3rem);
}
.btn:active {
  transform: translateY(-1px);
}

/* media queries */

@media (max-width:20000px) {
  .NavBar {
  background-color: #b2966f;
  height: 6rem;
  text-decoration: none;
  display: flex;
  align-items: center;
  width: 100%;
  z-index: 10;
  padding-right: 2rem;
}

.coffee {
  z-index: 10;
  margin-left: 4rem;
}

.btn {
   display: inline-block; 
   flex-flow: row; 
   justify-content: space-between; 
   margin-bottom: 1rem; 
   margin-left: 18rem; 
  font-size: 1.25rem;
  text-align: center;
  text-decoration: none;
  z-index: 10;
}

div {
  position: sticky;
  top: 0;
  margin-left: -1.5rem;
  z-index: 10;
}
}

@media (max-width:768px) {
  .NavBar {
  background-color: #b2966f;
  max-width: 100%;
  height: 7rem;
  text-decoration: none;
  align-items: center;
  z-index: 10;
}

.coffee {
  z-index: 10;
  margin-left: 1rem;
}

.btn {
  margin-top: 2rem;
  margin-bottom: 0rem;
  margin-left: 7%;
  font-size: 0.75rem;
  text-align: center;
  text-decoration: none;
  z-index: 10;
}

div {
  position: sticky;
  top: 0;
  margin-left: -1.5rem;
  z-index: 10;
}
}
@media (max-width:414px) {
  .NavBar {
  background-color: #b2966f;
  max-width: 10rem;
  height: 2rem;
  text-decoration: none;
  align-items: center;
  z-index: 10;
    margin-bottom: 3rem;
}

.coffee {
  z-index: 10;
  margin-left: 1.5rem;
}

.btn {
  margin-top: 2rem;
  margin-bottom: 0rem;
  margin-left: 1%;
  font-size: 0.5rem;
  text-align: center;
  text-decoration: none;
  z-index: 10;
}

div {
  position: sticky;
  top: 0;
  margin-left: -1.5rem;
  z-index: 10;
}
}

</style>

<script>
export default {
  navbar: Object,
}
</script>
