<script setup>
import City from '../components/City.vue'

const ville = {
  name: 'Ma ville',
  weather: 'Peu nuageux',
  temperature: 20.55,
  updatedAt: new Date()
}
</script>

<template>
    <h2>Météo - Liste des villes</h2>
    <City :name="ville.name"
          :temperature ="ville.temperature"
          :updatedAt="ville.updatedAt"
          :weather="ville.weather"
    />
</template>
