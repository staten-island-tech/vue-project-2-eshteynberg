<template>
  <div>
      <photospg></photospg>
  </div>
</template>

<script>
import photospg from '../components/photospg.vue'
export default {
  components: { photospg },

}
</script>

<style>
.light{
  background-color: var(--light-bg);
  color: var(--light-font);
}

.dark{
  background-color: var(--dark-bg);
  color: var(--dark-font)
}
</style>