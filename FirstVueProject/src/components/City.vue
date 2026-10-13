<script setup>
defineProps(['name', 'weather', 'temperature', 'updatedAt'])
</script>
<template>
    <div class="encadre">
    <h2>{{ name }}</h2>
        <p>Temps : {{ weather }}</p>
        <p>Température : {{ temperature }} °C</p>
        <p>Dernière mise à jour : {{ updatedAt?.toLocaleString() }}</p>
    </div>
</template>

<style scoped>
  .encadre {
    border: 1px solid #3498db;
    background-color: #f8f9fa;
    border-radius: 8px;
    padding: 16px;
    margin: 16px 0;
    box-shadow: 0 2px 4px rgba(0,0,0,0.05);
  }

  .encadre h2 {
    margin-top:0;
    color: #2c3e50;
  }
</style>
