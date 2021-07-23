<template>
  <div class="carta">
    <h5><span class="badge bg-light text-dark">Primer Componente</span></h5>
    <nav class="navbar navigation">
      <div class="container-fluid">
        <router-link to="/" class="ruta">INICIO</router-link>
        <div class="d-flex">
          <button @click="nextPages" class="btn btn-outline-light" >SIGUIENTE</button>
        </div>
      </div>
    </nav>
  </div>
</template>
<script>
export default {
    name: 'Navegacion',
    methods:{
        nextPages(){
            this.$router.push({name:'Vista'})
        }
    }
}
</script>

<style>
.carta{
  background-color: beige;
  border-radius: 5px;
  padding: 1rem;
}
  .navigation{
    background-color: rgb(76, 77, 77);
    border-radius: 5px;
  }
  .tituloComponente{
    background-color: white;
    padding: 2px;
  }
  .ruta{
    color: white;
    text-decoration: none;
  }
  .ruta:hover{
    color: burlywood;
  }
</style>