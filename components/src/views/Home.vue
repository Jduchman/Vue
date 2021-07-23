<template>
  <div class="home">
    <Detalle />
  </div>
</template>

<script>
// @ is an alias to /src
import Detalle from '@/components/Detalle.vue'

export default {
  name: 'Home',
  components: {
    Detalle,
  }
}
</script>

<style>
  .home{
    margin-top: 1rem;
  }
</style>