<template>
  <div class="home">
    <Detalle />
    <Formulario class="compForm"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Detalle from '@/components/Detalle.vue'
import Formulario from '@/components/Formulario.vue'

export default {
  name: 'Home',
  components: {
    Detalle,
    Formulario
  }
}
</script>

<style>
  .home{
    margin-top: 1rem;
  }
  .compForm{
      margin-top: 1rem;
  }
</style>