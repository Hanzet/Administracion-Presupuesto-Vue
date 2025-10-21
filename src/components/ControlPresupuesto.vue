<script setup>
import imagen from "../assets/img/grafico.jpg";
</script>

<template>
  <div class="dos-columnas">
    <div class="contenedor-grafico">
      <img :src="imagen" alt="imagen grafico" />
    </div>

    <div class="contenedor-presupuesto">
      <button class="reset-app">Resetear App</button>

      <p>
        <span>Presupuesto:</span>
        $0
      </p>

      <p>
        <span>Disponible:</span>
        $0
      </p>

      <p>
        <span>Gastado:</span>
        $0
      </p>
    </div>
  </div>
</template>

<style scoped>
.dos-columnas {
  display: flex;
  flex-direction: column;
}

.columnas-grafico > :first-child {
  margin-bottom: 3rem;
}

@media (min-width: 768px) {
  .dos-columnas {
    flex-direction: row;
    gap: 4rem;
    align-items: center;
  }
}
</style>
