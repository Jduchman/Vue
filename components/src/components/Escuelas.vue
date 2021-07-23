<template>
  <div class="card" v-for="(escuela, item) in escuelas" :key="item">
    <div class="card-header">
      {{ escuela.facultad }}
    </div>
    <div class="card-body cardB">
      <blockquote class="blockquote mb-0">
          <h2>{{escuela.nombre}}</h2>
        <p>{{escuela.descripcion}}</p>
        <footer class="blockquote-footer">
          <a :href="escuela.url">Visitar Sitio</a>
        </footer>
      </blockquote>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      escuelas: [
        {
          facultad: "Facultad de ciencias Agrarias",
          nombre: "Agronomía",
          descripcion:
            "Dolorum molestiaem sed quasi amet ad asperiores at consequuntur necessitatibus odio? Voluptatum, nisi corporis.",
          url: "https://www.unsch.edu.pe/facultades/agrarias/",
        },
        {
          facultad: "Facultad de ciencias Agrarias",
          nombre: "Ingenieria Agricola",
          descripcion:
            "Lorem, ipsum dolor sit amet comet ad asperiores at consequuntur necessitatibus odio? Voluptatum, nisi corporis.",

          url: "https://www.unsch.edu.pe/facultades/agrarias/",
        },
        {
          facultad: "Facultad de Ingenieria de Minas, Geologia y Civil",
          nombre: "Ing Sistemas",
          descripcion:
            "Lorem, ipsum dolor sit amet consectetur apellendus tempora a s at consequuntur necessitatibus odio? Voluptatum, nisi corporis.",

          url: "https://www.unsch.edu.pe/facultades/minas/",
        },
        {
          facultad: "Facultad de Ingenieria de Minas, Geologia y Civil",
          nombre: "Ing Civil",
          descripcion:
            "Lorem, ipsum m, magni repellendus tempora a rerum sed qu at consequuntur necessitatibus odio? Voluptatum, nisi corporis.",

          url: "https://www.unsch.edu.pe/facultades/minas/",
        },
      ],
    };
  },
};
</script>
<style>
    .cardB{
        background-color: beige;
    }
    .card-header{
        background-color:  rgb(76, 77, 77);
        color: white;
    }
</style>