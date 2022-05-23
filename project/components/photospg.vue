<template>
    <div>
        
            <img class="info-josh" src="./img/placeholder.png" alt="">
            <img class="info-emily" src="./img/placeholder.png" alt="">
            <img class="info-satina" src="./img/placeholder.png" alt="">
            <img class="info-whalen" src="./img/placeholder.png" alt="">
            <img class="quotePg" src="./img/This One.png" alt="">
            <a class="josh"  alt=""><img class="ph" src="./img/placeholder.png" alt=""></a>
            <a class="emily" alt=""><img class="ph" src="./img/placeholder.png" alt=""></a>
            <a class="satina" alt=""><img class="ph" src="./img/placeholder.png" alt=""></a>
            <a class="whalen" alt=""><img class="ph" src="./img/placeholder.png" alt=""></a>
            
    </div>

  
</template>

<style>
.quotePg{
    width: 117.9375rem;
    height: 60rem;
    z-index: -10000;
}

.ph{
    width: 10rem;
    height: 10rem;
    z-index: 0;
    opacity: 100%;
}

.satina{
    position: absolute;
    top: 18rem;
    left: 58.5rem;
    height: 15rem;
    width: 15rem;
}
.satina:hover ~ .info-satina{ 
    animation-name: fadeIn;
    animation-duration: 1s; 
}
.josh{
    position: absolute;
    top: 11rem;
    left: 20.5rem;
    height: 15rem;
    width: 15rem;
}
.josh:hover ~ .info-josh{ 
    animation: fadeIn 1s;
}
.emily{
    position: absolute;
    top: 26.25rem;
    left: 40rem;
    height: 15rem;
    width: 15rem;
}
.emily:hover ~ .info-emily{ 
    animation: fadeIn 1s; 
}
.whalen{
    position: absolute;
    top: 18rem;
    left: 82rem;
    height: 15rem;
    width: 15rem;
}
.whalen:hover ~ .info-whalen{ 
    animation-name: fadeIn;
    animation-duration: 1s; 
}

.info-josh{
     width: 15rem;
    height: 15rem;
    position: absolute;
    margin-top: 3rem;
    margin-left: 39rem;
}
.info-emily{
     width: 15rem;
    height: 15rem;
    position: absolute;
    margin-top: 3rem;
    margin-left: 39rem;
}
.info-satina{
     width: 15rem;
    height: 15rem;
    position: absolute;
    margin-top: 3rem;
    margin-left: 39rem;
}
.info-whalen{
     width: 15rem;
    height: 15rem;
    position: absolute;
    margin-top: 3rem;
    margin-left: 39rem;
}

@keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

</style>