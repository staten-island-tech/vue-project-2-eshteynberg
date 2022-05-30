<template>
  <div>
    <img class="map" src="/img/map.png" alt="map of the world" />

    <div class="pin">
      <a class="pin-america" href="/amer"
        ><img class="btn-img-pin" src="/img/pin.png" alt="Pin on American"
      /></a>
      <a class="pin-korea" href="/korea"
        ><img class="btn-img-pin" src="/img/pin.png" alt="Pin on Korea"
      /></a>
      <a class="pin-italy" href="/italy"
        ><img class="btn-img-pin" src="/img/pin.png" alt="Pin on Italy"
      /></a>
      <a class="pin-mexico" href="/mex"
        ><img class="btn-img-pin" src="/img/pin.png" alt="Pin on Mexico"
      /></a>
      <img class="hov-amer" src="../static/img/american food.jpg" alt="image shows up after hovering over pin on america" />
      <img class="hov-kor" src="../static/img/asian.png" alt="image shows up after hovering over pin on korea" />
      <img class="hov-ita" src="../static/img/mediterranean food.jpg" alt="image shows up after hovering over pin on italy" />
      <img class="hov-mex" src="../static/img/spanish food.jpg" alt="image shows up after hovering over pin on mexico" />
    </div>
  </div>
</template>

<script>
import FilteredPosts from './FilteredPosts.vue'
export default {
  components: { FilteredPosts },
}
</script>

<style>
.pin-america:hover {
  transform: translateY(-0.3rem);
}
.pin-america:active {
  transform: translateY(-1px);
}
.pin-america:hover ~ .hov-amer {
  animation: fadeIn 1s;
  animation-fill-mode: forwards;
}

.pin-korea:hover {
  transform: translateY(-0.3rem);
}
.pin-korea:active {
  transform: translateY(-1px);
}
.pin-korea:hover ~ .hov-kor {
  animation: fadeIn 1s;
  animation-fill-mode: forwards;
}

.pin-mexico:hover {
  transform: translateY(-0.3rem);
}
.pin-mexico:active {
  transform: translateY(-1px);
}
.pin-mexico:hover ~ .hov-mex {
  animation: fadeIn 1s;
  animation-fill-mode: forwards;
}

.pin-italy:hover {
  transform: translateY(-0.3rem);
}
.pin-italy:active {
  transform: translateY(-1px);
}
.pin-italy:hover ~ .hov-ita {
  animation: fadeIn 1s;
  animation-fill-mode: forwards;
}

.light{
  background-color: var(--light-bg);
  color: var(--light-font);
}

.dark{
  background-color: var(--dark-bg);
  color: var(--dark-font)
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

@media (max-width: 20000px) {
  .map {
    height: 57.5rem;
    width: 1903px;
  }

  .pin-america {
    position: absolute;
    top: 30rem;
    left: 22.25rem;
    height: 5rem;
    width: 5rem;
  }

  .pin-korea {
    position: absolute;
    top: 30.5rem;
    left: 93rem;
    height: 5rem;
    width: 5rem;
  }

  .pin-mexico {
    position: absolute;
    top: 33.75rem;
    left: 20.5rem;
    height: 5rem;
    width: 5rem;
  }

  .pin-italy {
    position: absolute;
    top: 29rem;
    left: 57rem;
    height: 5rem;
    width: 5rem;
  }

  .hov-amer {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 24.5rem;
    left: 21.25rem;
    opacity: 0;
  }
  .hov-kor {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 25rem;
    left: 92rem;
    opacity: 0;
  }
  .hov-ita {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 23.5rem;
    left: 56rem;
    opacity: 0;
  }
  .hov-mex {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 28.75rem;
    left: 15rem;
    opacity: 0;
  }

  .btn-img-pin {
    height: 3rem;
    position: relative;
  }
}

@media (max-width: 768px) {
  .map {
    max-width: 47rem;
    height: 27rem;
  }

  .pin-america {
    position: absolute;
    top: 18rem;
    left: 8rem;
    height: 5rem;
    width: 5rem;
  }

  .pin-korea {
    position: absolute;
    top: 18rem;
    left: 36.5rem;
    height: 5rem;
    width: 5rem;
  }

  .pin-mexico {
    position: absolute;
    top: 19.75rem;
    left: 7.5rem;
    height: 5rem;
    width: 5rem;
  }

  .pin-italy {
    position: absolute;
    top: 17.25rem;
    left: 22rem;
    height: 5rem;
    width: 5rem;
  }

  .hov-amer {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 24.5rem;
    left: 21.25rem;
    opacity: 0;
  }
  .hov-kor {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 25rem;
    left: 92rem;
    opacity: 0;
  }
  .hov-ita {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 23.5rem;
    left: 56rem;
    opacity: 0;
  }
  .hov-mex {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 28.75rem;
    left: 15rem;
    opacity: 0;
  }

  .btn-img-pin {
    height: 2rem;
    position: relative;
  }
}
@media (max-width: 414px) {
  .map {
    max-width: 25rem;
    height: 20rem;
  }

  .pin-america {
    position: absolute;
    top: 12.5rem;
    left: 4rem;
    height: 5rem;
    width: 5rem;
  }

  .pin-korea {
    position: absolute;
    top: 12.5rem;
    left: 18.75rem;
    height: 5rem;
    width: 5rem;
  }

  .pin-mexico {
    position: absolute;
    top: 14.5rem;
    left: 3.5rem;
    height: 5rem;
    width: 5rem;
  }

  .pin-italy {
    position: absolute;
    top: 12.25rem;
    left: 11rem;
    height: 5rem;
    width: 5rem;
  }

  .hov-amer {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 24.5rem;
    left: 21.25rem;
    opacity: 0;
  }
  .hov-kor {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 25rem;
    left: 92rem;
    opacity: 0;
  }
  .hov-ita {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 23.5rem;
    left: 56rem;
    opacity: 0;
  }
  .hov-mex {
    height: 5rem;
    width: 5rem;
    position: absolute;
    top: 28.75rem;
    left: 15rem;
    opacity: 0;
  }

  .btn-img-pin {
    height: 2rem;
    position: relative;
  }
}
</style>