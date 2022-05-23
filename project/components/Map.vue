<template>
<div>

<img class="map" src="./img/map.png" alt="">

<div class="pin">
    <a class="pin-america" href="/onePost"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>
    <a class="pin-korea" href="/onePost"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>
    <a class="pin-italy" href="/onePost"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>
    <a class="pin-mexico" href="/onePost"><img class="btn-img-pin" src="./img/pin.png" alt=""></a>


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
.map{
    height: 57.5rem;
    width: 116.625rem;
}

.pin-america{
    position: absolute;
    top: 30rem;
    left: 21.25rem;
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
animation: fadeIn 1s;
}
@keyframes fadeIn {
  0% {opacity:1;}
  100% {opacity:0;}
}


.pin-korea{
    position: absolute;
    top: 30.5rem;
    left: 92rem;
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
animation: fadeIn 1s; 
}
@keyframes fadeIn {
  0% {opacity:100%;}
  100% {opacity:0%;}
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
.pin-italy:hover ~ .pin-america{
animation: fadeIn 1s;
}
@keyframes fadeIn {
  0% {opacity:1;}
  100% {opacity:0;}
}

.pin-mexico{
    position: absolute;
    top: 34.25rem;
    left: 20.5rem;
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
animation: fadeIn 1s; 
}
@keyframes fadeIn {
  0% {opacity:1;}
  100% {opacity:0;}
}

.btn-img-pin {
 height: 3rem;
 position: relative;
 margin-right: 98rem;
}
</style>