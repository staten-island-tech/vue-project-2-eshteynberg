<template>
  <div>

<img class="map" src="./img/map.png" alt="">

<div class="pin">
    <a class="pin-america" href="/amer"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>
    <a class="pin-korea" href="/korea"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>
    <a class="pin-italy" href="/italy"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>
    <a class="pin-mexico" href="/mex"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>
    <img class="hov-amer" src="./img/placeholder.png" alt="">
    <img class="hov-kor" src="./img/placeholder.png" alt="">
    <img class="hov-ita" src="./img/placeholder.png" alt="">
    <img class="hov-mex" src="./img/placeholder.png" alt="">


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

.map {
  height: 57.5rem;
  width: 120rem;
}

.pin-america {
  position: absolute;
  top: 30rem;
  left: 21.25rem;
  height: 5rem;
  width: 5rem;
}
.pin-america:hover {
  transform: translateY(-0.3rem);
}
.pin-america:active {
  transform: translateY(-1px);
}
.pin-america:hover ~ .hov-amer{
animation: fadeIn 1s;
animation-fill-mode: forwards;
}

.pin-korea{
    position: absolute;
    top: 30.5rem;
    left: 92rem;
    height: 5rem;
    width: 5rem;
}
.pin-korea:hover {
  transform: translateY(-0.3rem);
}
.pin-korea:active {
  transform: translateY(-1px);
}
.pin-korea:hover ~ .hov-kor{
animation: fadeIn 1s; 
animation-fill-mode: forwards;
}


.pin-mexico{
    position: absolute;
    top: 33.75rem;
    left: 19rem;
    height: 5rem;
    width: 5rem;
}
.pin-mexico:hover {
  transform: translateY(-0.3rem);
}
.pin-mexico:active {
  transform: translateY(-1px);
}
.pin-mexico:hover ~ .hov-mex{
animation: fadeIn 1s; 
animation-fill-mode: forwards;
}

.pin-italy{
    position: absolute;
    top: 29rem;
    left: 56rem;
    height: 5rem;
    width: 5rem;
}
.pin-italy:hover{
  transform: translateY(-0.3rem);
}
.pin-italy:active {
  transform: translateY(-1px);
}
.pin-italy:hover ~ .hov-ita{
animation: fadeIn 1s;
animation-fill-mode: forwards;
}

.hov-amer{ 
  height: 5rem;
  width: 5rem;
  position: absolute;
    top: 24.5rem;
    left: 21.25rem;
  opacity: 0;
}
.hov-kor{ 
  height: 5rem;
  width: 5rem;
  position: absolute;
    top: 25rem;
    left: 92rem;
  opacity: 0;
}
.hov-ita{ 
  height: 5rem;
  width: 5rem;
  position: absolute;
    top: 23.5rem;
    left: 56rem;
  opacity: 0;
}
.hov-mex{ 
  height: 5rem;
  width: 5rem;
  position: absolute;
    top: 28.75rem;
    left: 15rem;
  opacity: 0;
}

@keyframes fadeIn {
  0% {
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}

.btn-img-pin {
  height: 3rem;
  position: relative;
  margin-right: 98rem;
}
</style>