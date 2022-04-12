<template>
    <div class="NavBar">
        <img class="coffee" src="./img/coffee.png" alt="">
        <a class="btn" href='\pages\index.vue'>Home</a>
        <a class="btn" href='/about'>About</a>
        <a class="btn" href='/cuisines'>Cuisines</a>
        <a class="btn">Contact Us</a>
        
    </div>
</template>

<style scoped>
.NavBar{
    background-color: #B2966F;
    height: 6rem;
}

.coffee{ 
    z-index: -1;
    margin-left: 3rem;
}

.btn    {
    display: inline-block;
    background-color: #B2966F;
    color: white;
    flex-flow: row;
    justify-content: space-between;
    margin-bottom: 1rem;
    margin-left: 18rem;
    border: #B2966F solid ;
    font-size: 1.25rem;
    text-align: center;
}
</style>

<script>
export default {
    navbar: Object,
}
</script>
