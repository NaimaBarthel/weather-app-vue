<script setup>
       const onListClick = () => {
       alert('Je veux voir la liste')
       };
</script>

<template>
    <h1>Météo des villes</h1>
    <!-- Le lien de navigation -->
    <nav>
        <router-link to="/">Accueil</router-link> |
        <router-link to="/villes" >Voir la liste des villes</router-link> |
        <router-link to="/ville" >Ma ville</router-link>
    </nav>
    <!-- La zone d'affichage de la route active -->
    <router-view></router-view>

    <!-- Intégration du composant CitiesList -->
    <!-- CitiesList/ -->
</template>

<style scoped></style>
