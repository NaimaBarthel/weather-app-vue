<script setup>
    const city = {
        name: 'Ma ville',
        weather: 'Peu nuageux',
        temperature: 20.55,
        updatedAt: new Date(),
    };
</script>
<template>
    <div>
    <h2>{{ city.name }}</h2>
        <p>Temps : {{ city.weather }}</p>
        <p>Température : {{ city.temperature }} °C</p>
        <p>Dernière mise à jour : {{ city.updatedAt.toLocaleString() }}</p>
    </div>
</template>
