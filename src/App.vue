<template>
  <div id="app">
    <div class="mr-4 ml-4 mb-5">
      <seccion-noticias></seccion-noticias>
    </div>
  </div>
</template>

<script>
import SeccionNoticias from "./components/SeccionNoticias.vue";

export default {

  name: "App",
  components: { SeccionNoticias },
  data(){
    return {
     

      equipo:[

    { 
      codigo:1,
      nombre: "Nombre del miembro de equipo",
      descripcion: "Lorem ipsum dolor sit amet, consectetur adipiscingelit. Mauris condimentum ac elit et accumsan.",
      rol:"Desarrolador backend",
      image:"/src/assets/logo.png",
    },
    { 
      codigo:1,
      nombre: "Nombre del miembro de equipo",
      descripcion: "Lorem ipsum dolor sit amet, consectetur adipiscingelit. Mauris condimentum ac elit et accumsan.",
      rol:"Desarrolador backend",
      image:"/src/assets/logo.png",
    },
    { 
      codigo:1,
      nombre: "Nombre del miembro de equipo",
      descripcion: "Lorem ipsum dolor sit amet, consectetur adipiscingelit. Mauris condimentum ac elit et accumsan.",
      rol:"Desarrolador backend",
      image:"/src/assets/logo.png",
    },
    { 
      codigo:1,
      nombre: "Nombre del miembro de equipo",
      descripcion: "Lorem ipsum dolor sit amet, consectetur adipiscingelit. Mauris condimentum ac elit et accumsan.",
      rol:"Desarrolador backend",
      image:"/src/assets/logo.png",
    },
    { 
      codigo:1,
      nombre: "Nombre del miembro de equipo",
      descripcion: "Lorem ipsum dolor sit amet, consectetur adipiscingelit. Mauris condimentum ac elit et accumsan.",
      rol:"Desarrolador backend",
      image:"/src/assets/logo.png",
    }

      ]

      }
  }
};
</script>
