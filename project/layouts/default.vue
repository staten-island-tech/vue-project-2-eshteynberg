<template>
  <div class="container">
    <NavBar />
    <Nuxt />
  </div>
</template>

<script>
export default {}
</script>

<style >

.parent {
  display: grid;
  grid-template: auto 1fr auto / auto 1fr auto;
}

.container{ 
  z-index: 10000;
}

</style>