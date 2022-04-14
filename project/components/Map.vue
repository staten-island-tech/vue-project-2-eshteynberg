<template>
<div>

<img class="map" src="./img/map.png" alt="">

<div class="pin">
<button id="america" style="" class="pin-america"><img class="btn-img-pin" src="./img/pin.png" alt=""></button>
<button class="pin-korea"><img class="btn-img-pin" src="./img/pin.png" alt=""></button>
<button class="pin-italy"><img class="btn-img-pin" src="./img/pin.png" alt=""></button>
<button class="pin-mexico"><img class="btn-img-pin" src="./img/pin.png" alt=""></button>

</div>

</div>
</template>

<script>
export default {

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
    left: 20rem;
    height: 5rem;
    width: 5rem;
    color: transparent;
     background-color: transparent; 
     /* border-color: transparent;  */
}
.pin-korea{
    position: absolute;
    top: 30rem;
    left: 92rem;
    height: 5rem;
    width: 5rem;
    color: transparent;
     background-color: transparent; 
     /* border-color: transparent;  */
}
.pin-italy{
    position: absolute;
    top: 30rem;
    left: 57rem;
    height: 5rem;
    width: 5rem;
    color: transparent;
     background-color: transparent; 
     /* border-color: transparent;  */
}
.pin-mexico{
    position: absolute;
    top: 35rem;
    left: 21rem;
    height: 5rem;
    width: 5rem;
    color: transparent;
     background-color: transparent; 
     /* border-color: transparent;  */
}

.btn-img-pin {
 height: 2rem;
 position: relative;
 margin-right: 100rem;
}
</style>