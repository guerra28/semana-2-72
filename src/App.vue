<template>
  <div id="app">
    <div class="mr-4 ml-4 mb-5">
      <seccion-noticias></seccion-noticias>
    </div>
    <div class="container-fluid">
      <team-card :member="equipo"> </team-card>
    </div>
  </div>
</template>

<script>
import SeccionNoticias from "./components/SeccionNoticias.vue";
import TeamCard from "./components/TeamCard.vue";

export default {
  name: "App",
  components: { SeccionNoticias, TeamCard },

  data() {
    return {
      equipo: [
        {
          codigo: 1,
          nombre: "Emerson David Cardona Marín",
          descripcion:
            "Edad: 47 años Ciudad de residencia: Dosquebradas  Ocupación: Docente Universitario Universidad Tecnológica de Pereira",
          rol: "Desarrolador backend",
          image: require("./assets/avatar-david.jpg"),
        },
        {
          codigo: 2,
          nombre: "Andrés Felipe Figueroa Betancourt",
          descripcion:
            "Edad: 24 años  Ciudad de residencia: Bogotá  Ocupación: Estudiante de Maestría",
          rol: "Desarrolador backend",
          image: require("./assets/avatar-andres.png"),
        },
        {
          codigo: 3,
          nombre: "Juan Álvaro Guerra Sánchez",
          descripcion:
            "Edad: 27 años Ciudad de residencia: Manizales Ocupación: Asesor de atención al cliente",
          rol: "Desarrolador backend",
          image: require("./assets/avatar-juan.jpeg"),
        },
        {
          codigo: 4,
          nombre: "Daniel José Montoya Sánchez",
          descripcion:
            "Edad: 26 años Ciudad de residencia: Medellín Ocupación: Estudiante de Ingeniería",
          rol: "Desarrolador backend",
          image: require("./assets/avatar-daniel.png"),
        },
        {
          codigo: 5,
          nombre: "Yeimy Xiomara Torres Sánchez",
          descripcion:
            "Ciudad de residencia: Bogotá Ocupación: Ingeniera Industrial",
          rol: "Desarrolador backend",
          image: require("./assets/avatar-xiomara.jpeg"),
        },
      ],
    };
  },
};
</script>
