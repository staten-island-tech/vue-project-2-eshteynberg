<template>
<div>

<img class="map" src="./img/map.png" alt="">

<div class="pin">
    <a class="pin-america" href="/onePost"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>
    <a class="pin-korea" href="/onePost"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>
    <a class="pin-italy" href="/onePost"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>
    <a class="pin-mexico" href="/onePost"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>


</div>
<filtered-posts></filtered-posts>
</div>
</template>

<script>
import FilteredPosts from './FilteredPosts.vue'
export default {
  components: { FilteredPosts },

}

</script>

<style>
.map{
    height: 57.5rem;
    width: 115.625rem;
}

.pin-america{
    position: absolute;
    top: 30rem;
    left: 21.5rem;
    height: 5rem;
    width: 5rem;
}
.pin-america:hover{
  transform: translateY(-0.3rem);
}
.pin-america:active {
  transform: translateY(-1px);
}
.pin-america:hover ~ .pin-italy{
animation: fadein 1s; 
}
@keyframes fadeIn {
  100% {opacity:1;}
  1% {opacity:0;}
}


.pin-korea{
    position: absolute;
    top: 30rem;
    left: 90.5rem;
    height: 5rem;
    width: 5rem;
}
.pin-korea:hover{
  transform: translateY(-0.3rem);
}
.pin-korea:active {
  transform: translateY(-1px);
}
.pin-korea:hover ~ .pin-italy{
animation: fadein 1s; 
}
@keyframes fadeIn {
  100% {opacity:1;}
  1% {opacity:0;}
}

.pin-italy{
    position: absolute;
    top: 29rem;
    left: 55.5rem;
    height: 5rem;
    width: 5rem;
    opacity: 100%;
}
.pin-italy:hover{
  transform: translateY(-0.3rem);
}
.pin-italy:active {
  transform: translateY(-1px);
}
.pin-italy:hover ~ .pin-italy{
animation: fadein 1s; 
}
@keyframes fadeIn {
  100% {opacity:1;}
  1% {opacity:0;}
}

.pin-mexico{
    position: absolute;
    top: 34rem;
    left: 20rem;
    height: 5rem;
    width: 5rem;
}
.pin-mexico:hover{
  transform: translateY(-0.3rem);
}
.pin-mexico:active {
  transform: translateY(-1px);
}
.pin-mexico:hover ~ .pin-italy{
animation: fadein 1s; 
}
@keyframes fadeIn {
  100% {opacity:1;}
  1% {opacity:0;}
}

.btn-img-pin {
 height: 3rem;
 position: relative;
 margin-right: 98rem;
}
</style>