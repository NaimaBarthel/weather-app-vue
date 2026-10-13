<script setup>
import City from '../components/City.vue'

const cities =
    [{
      id: 1,
      name: 'Ville 1',
      weather: 'Ensoleillé',
      temperature: 22.0,
      updatedAt: new Date()
    },
    {
      id: 2,
      name: 'Ville 2',
      weather: 'Peu nuageux',
      temperature: 19.5,
      updatedAt: new Date()
    }]

</script>

<template>
    <h2>Météo - Liste des villes</h2>
    <City
        v-for="ville in cities" :key="ville.id"
                                :name="ville.name"
                                :temperature ="ville.temperature"
                                :updatedAt="ville.updatedAt"
                                :weather="ville.weather"
    />
</template>
