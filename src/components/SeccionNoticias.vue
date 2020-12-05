<template>
  <div class="row mt-5 mb-3">
    <div
      class="col-sm-6 mb-3 mr-auto"
      v-for="(noticia, index) in noticias"
      :key="index"
    >
      <div class="card">
      <img :src="noticia.urlToImage" class="img-fluid mt-2 ml-2 mr-2" alt="imagen" />
        <div class="card-body">
          <h5 class="card-title">{{ noticia.title }}</h5>
          <h6 class="card-sub-title">
            {{ noticia.publishedAt }}
          </h6>
          <p class="card-text">
            {{ noticia.content }}
          </p>
          <a :href="noticia.url" class="btn btn-primary" target="_blank">Leer más-></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "SeccionNoticias",
  data() {
    return {
      noticias: null,
    };
  },

  mounted() {
    axios
      .get(
        "http://newsapi.org/v2/top-headlines?country=co&apiKey=fde1d3d6e53548e880c54df54924a946"
      )

      .then((response) => {
        this.noticias = response.data.articles.slice(0, 4);

        
      });
  },
};
</script>

<style scoped>
</style>