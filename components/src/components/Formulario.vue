<template>
  <div class="carta">
    <div class="card-body">
      <form action="" @submit.prevent="agregarUser">
        <div class="input-group mb-3">
          <input
            type="text"
            class="form-control"
            v-model="nombreUser"
            placeholder="Username"
            aria-label="Recipient's username"
            aria-describedby="button-addon2"
          />
          <div class="input-group-append">
            <button
              class="btn btn-outline-secondary"
              @click="limpiar"
              id="button-addon2"
            >
              X
            </button>
            <button
              class="btn btn-outline-secondary"
              type="submit"
              id="button-addon2"
            >
              Agregar
            </button>
          </div>
        </div>
        <div v-show="showAlert" class="alert alert-info" role="alert">
          Dato ingresado correctamente
        </div>
      </form>
      <h3>Dato Usuario</h3>
      <p style="color: red">{{ nombreUser }}</p>
    </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            nombreUser: "",
            showAlert: false
        }
    },

    methods: {
        agregarUser(){
            if(!this.nombreUser == "")
                this.showAlert = true
        },
        limpiar(){
            this.nombreUser = ""
            this.showAlert = false
        }
    },
}
</script>