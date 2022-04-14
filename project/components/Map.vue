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
    top: 32rem;
    left: 23rem;
    height: 5rem;
    width: 5rem;
}
.pin-korea{
    position: absolute;
    top: 32rem;
    left: 92rem;
    height: 5rem;
    width: 5rem;
}
.pin-italy{
    position: absolute;
    top: 30rem;
    left: 57rem;
    height: 5rem;
    width: 5rem;
}
.pin-mexico{
    position: absolute;
    top: 36rem;
    left: 21.5rem;
    height: 5rem;
    width: 5rem;

}

.btn-img-pin {
 height: 2rem;
 position: relative;
 margin-right: 100rem;
}
</style>