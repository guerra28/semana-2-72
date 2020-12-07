<template>
  <div class="card-deck">
    <div class="card" v-for="(miembro, index) in member" :key="index">
      <img :src="miembro.image" class="card-img-top mg-fluid" alt="..." />

      <div class="card-body">
        <h5 class="card-title">{{ miembro.nombre }}</h5>
        <p class="card-text">
          {{ miembro.descripcion }}
        </p>
        <p class="card-text">
          <small class="text-muted"><span>Rol: </span>{{ miembro.rol }} </small>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TeamCard",
  props: ["member"],
};
</script>

<style scoped></style>
