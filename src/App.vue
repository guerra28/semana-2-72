<template>
  <div id="app">
    <div class="container-fluid"> 
      <section-api></section-api>
    </div>
  
    <div class="container-fluid"> 
      <div class="row justify-content-center mb-5"> 
        <div class="col mt-5" v-for=" (item, index) of member" :key="index">
          <team-card v-bind:member="item"> </team-card>
        </div> 
      </div>
    </div>

    <section-footer></section-footer>
  </div>
</template>

<script>
import SectionFooter from "./components/SectionFooter.vue";
import TeamCard from "./components/TeamCard.vue";
import SectionApi from "./components/SectionApi.vue";
import team from "../public/team.json";

export default {
  name: "App",
  components: {
    SectionFooter,
    TeamCard,
    SectionApi,
  },
  data() {
    return {
      member: team.team
    }
  }
}
</Script>
