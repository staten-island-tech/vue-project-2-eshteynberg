<template>
<div>
    <img id="trees" src="./img/trees.png" alt="">
    <img id="chalk" src="./img/chalk.png" alt="">
    <img id="dots" src="./img/dots.png" alt="">
    <h1 id="food-blog">SATINA'S</h1>
    <h1 id="food-blog"> FOOD BLOG</h1>
</div>

</template>

<style scoped>
#chalk {
    position: absolute;
    top: 1rem;
    left: 25%;
}

#trees { 
position:  relative;
top: 5rem
}

#dots { 
position:  absolute;
top: 0%;
z-index: -1;
height: 80rem;
width: 100%;
}

#food-blog{
    position: relative;
    bottom: 60rem;
    text-align: center;
    font-size: 4rem;
    color: white;
}

</style>