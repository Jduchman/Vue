<template>
  <div id="nav">
    <Navegacion />
  </div>
  <router-view/>
</template>

<script>

import Navegacion from '@/components/Navegacion.vue'

export default {
  components:{
    Navegacion
  }
}
</script>

<style>
  html{
    margin: 2rem 10rem;
    }
</style>
