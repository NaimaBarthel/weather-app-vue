<script setup>
import CitiesList from './views/CitiesList.vue';

       const onListClick = () => {
       alert('Je veux voir la liste')
       };
</script>

<template>
    <h1>Météo des villes</h1>
    <button @click="onListClick">Voir la liste</button>

    <!-- Intégration du composant CitiesList -->
    <CitiesList/>
</template>

<style scoped></style>
