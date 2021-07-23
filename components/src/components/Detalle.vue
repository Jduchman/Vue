<template>
  <div class="carta">
    <h5><span class="badge bg-light text-dark">Segundo Componente</span></h5>
    <div class="contenedorUnsch">
        <h3>UNIVERSIDAD NACIONAL SAN CRISTOBAL DE HUAMANGA</h3>
        <div v-if="true" class="ubicacion">
            <h3>AYACUCHO-PERU</h3>
        </div>
        <div class="botones">
            <button @click="verDetalle" class="btn btn-success">Mostrar Detalle</button>
        </div>
        <Oculto v-if="detalleOculto" />
    </div>
  </div>
</template>

<script>

import Oculto from '@/components/Oculto.vue'
export default {
    components:{
        Oculto
    },

    data() {
        return {
            detalleOculto: false,
        }
    },
    methods:{
        verDetalle(){
            this.detalleOculto = !this.detalleOculto;
        },
    }
}
</script>


<style>
    .botones{
        padding: 0 40%;
    }
</style>
