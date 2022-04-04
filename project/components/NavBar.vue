<template>
    <div class="NavBar">
        <button class="btn">Home</button>
        <button class="btn">About</button>
        <button class="btn">Cuisines</button>
        <button class="btn">Contact Us</button>
    </div>
</template>

<style scoped>
.NavBar{
    background-color: #B2966F;
    height: 6rem;
}

.btn    {
    display: inline-block;
    background-color: #B2966F;
    color: white;
    flex-flow: row;
    justify-content: space-between;
    margin-top: 1.5%;
    margin-left: 15%;
    border: #B2966F solid ;
    font-size: 1.25rem;
    text-align: center;
}
</style>