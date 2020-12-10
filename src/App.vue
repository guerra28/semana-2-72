<template>
  <div id="app">
    <div class="mr-4 ml-4 mb-5">
      <seccion-noticias></seccion-noticias>
    </div>

    <div class="container-fluid" id="nosotros"> 
      <div class="row justify-content-center mb-5"> 
        <div class="col mt-5" v-for=" (item, index) of member" :key="index">
          <team-card v-bind:member="item"> </team-card>
        </div> 
      </div>
    </div>
      
    <seccionFooter id="contacto"> </seccionFooter>
  </div>
</template>

<script>
import SeccionNoticias from "./components/SeccionNoticias.vue";
import TeamCard from "./components/TeamCard.vue";
import SeccionFooter from "./components/SeccionFooter.vue";
import team from "../public/team.json";

export default {
  name: "App",
  components: { SeccionNoticias, 
  TeamCard,
  SeccionFooter, },

  data() {
    return {
      member:team.team
    }
  },
};
</script>
