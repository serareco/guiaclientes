<template>
  <div class="card">
    <div class="card-body">
      <h5 class="card-title">{{ datos.description }}</h5>
      <h6 class="card-subtitle mb-2 text-muted">{{ datos.responsable }}</h6>
      <p class="card-text">{{ datos.detail }}</p>
      <a href="#" class="card-link">Resuelto</a>
      <a href="#" class="card-link">Postponer</a>
      <a href="#" class="card-link">Rechazar</a>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  props: {
    datos: Object,
  },
};
</script>

<style scoped>
</style>