<template>
  <div>
    <client-only><NavBar class="nav" /></client-only>
    
    <Nuxt />
  </div>
</template>

<script>
export default {}
</script>

<style >
.container {
  z-index: 10000;
}
*/ .nav {
  justify-items: center;
  padding-right: auto;
}



.theme-light {
background-color: var(--light-back);
  }
  .theme-dark {
background-color: var(--dark-back);
  }

</style>