<template>
  <div>
    <img class="quotePg" src="/img/This One.png" alt="Picture of Satina, Mr. Whalen, Emily, and a monkey" />
    <a class="josh" href="/about-j" alt="monkey">
      <img class="ph" src="/img/placeholder.png" alt="monkey">
      </a>
    <a class="emily" href="/about-e" alt="brian"
      ><img class="ph" src="/img/placeholder.png" alt="brian"
    ></a>
    <a class="satina" href="/about-s" alt="snorlaz"
      ><img class="ph" src="/img/placeholder.png" alt="snorlax"
   ></a>
    <a class="whalen" href="/about-w" alt="shiny"
      ><img class="ph" src="/img/placeholder.png" alt="shiny"
    ></a>
  </div>
</template>

<style>

@media (max-width:20000px) {
  
.light{
  background-color: var(--light-bg);
  color: var(--light-font);
}

.dark{
  background-color: var(--dark-bg);
  color: var(--dark-font)
}

.quotePg {
  width: 117.9375rem;
  height: 60rem;
  z-index: -10000;
}

.ph {
  width: 15rem;
  height: 15rem;
  z-index: 0;
  opacity: 0;
}

.satina {
  position: absolute;
  top: 18rem;
  left: 58.5rem;
  height: 15rem;
  width: 15rem;
  opacity: 100%;
}

.josh {
  position: absolute;
  top: 11rem;
  left: 20.5rem;
  height: 15rem;
  width: 15rem;
  opacity: 100%;
}

.emily {
  position: absolute;
  top: 26.25rem;
  left: 40rem;
  height: 15rem;
  width: 15rem;
  opacity: 100%;
}

.whalen {
  position: absolute;
  top: 18rem;
  left: 82rem;
  height: 15rem;
  width: 15rem;
  opacity: 100%;
}

}
@media (max-width:768px) {
  
.quotePg {
  max-width: 45rem;
  height: 28rem;
  z-index: -10000;
  margin-left: 1rem;
}

.ph {
  width: 5rem;
  height: 5rem;
  z-index: 0;
  opacity: 0;
}

.satina {
  position: absolute;
  top: 13rem;
  left: 23.5rem;
  height: 15rem;
  width: 15rem;
}

.josh {
  position: absolute;
  top: 11rem;
  left: 9.5rem;
  height: 15rem;
  width: 15rem;
}

.emily {
  position: absolute;
  top: 16.25rem;
  left: 17rem;
  height: 15rem;
  width: 15rem;
}

.whalen {
  position: absolute;
  top: 14rem;
  left: 32rem;
  height: 15rem;
  width: 15rem;
}

}
@media (max-width: 414px) {
  
.quotePg {
  max-width: 48rem;
  z-index: -10000;
  margin-left: 2rem;
}

.ph {
  width: 3rem;
  height: 3rem;
  z-index: 0;
  opacity: 0;
}

.satina {
  position: absolute;
  top: 9rem;
  left: 11.5rem;
  height: 15rem;
  width: 15rem;
}

.josh {
  position: absolute;
  top: 7rem;
  left: 4rem;
  height: 15rem;
  width: 15rem;
}

.emily {
  position: absolute;
  top: 11rem;
  left: 8rem;
  height: 15rem;
  width: 15rem;
}

.whalen {
  position: absolute;
  top: 9rem;
  left: 16rem;
  height: 15rem;
  width: 15rem;
}

}

</style>