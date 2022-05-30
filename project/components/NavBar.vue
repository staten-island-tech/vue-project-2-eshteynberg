<template>
  <div class="NavBar">
    <img class="coffee" src="/img/coffee.png" alt="nice picture of coffee" />
    <a class="btn" href="/">Home</a>
    <a class="btn" href="/about">About</a>
    <a class="btn" href="/cuisines">Cuisines</a>
    <a class="btn" href="/contact">Contact Us</a>
    <button onclick="body.className = ''; body.classList.add(`dark`)" class="btn theme">Dark Theme</button>
    <button onclick="body.className = ''; body.classList.add(`light`)" class="btn theme">Light Theme</button>
  </div>
</template>

<style scoped>
.btn{
  color: var(--post);
}
.btn:hover {
  transform: translateY(-0.3rem);
}
.btn:active {
  transform: translateY(-1px);
}

.theme {
    background:none;
    border:none;
    margin:0;
    padding:0;
    cursor: pointer;
}

.light{
  background-color: var(--light-bg);
  color: var(--light-font);
}

.dark{
  background-color: var(--dark-bg);
  color: var(--dark-font)
}

/* media queries */

@media (max-width:20000px) {
  .NavBar {
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
   margin-left: 11%; 
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
  max-width: 100%;
  height: 7rem;
  text-decoration: none;
  align-items: center;
  z-index: 10;
}

.coffee {
  z-index: 10;
  margin-left: 3rem;
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
  max-width: 30rem;
  height: 2rem;
  text-decoration: none;
  align-items: center;
  z-index: 10;
    margin-bottom: 3rem;
}

.coffee {
  z-index: 10;
  margin-left: 2rem;
  width: 3rem;
}

.btn {
  margin-top: 2rem;
  margin-bottom: 1rem;
  margin-left: 7%;
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
  props:
  {
  navbar: Object,  
  },
  methods: {
  myFunction() {
    console.log('eggs')
  },
}
}





</script>
