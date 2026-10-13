<script setup>
defineProps(['name', 'weather', 'temperature', 'updatedAt'])
</script>
<template>
    <div>
    <h2>{{ name }}</h2>
        <p>Temps : {{ weather }}</p>
        <p>Température : {{ temperature }} °C</p>
        <p>Dernière mise à jour : {{ updatedAt?.toLocaleString() }}</p>
    </div>
</template>
