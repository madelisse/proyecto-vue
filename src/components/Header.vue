<template>
    <div class="header">
        <h3>La temperatura actual es: <Weather></Weather> </h3>
    </div>
</template>
<script setup>
    import Weather from './Weather.vue';
</script>
<style scoped>
    .header {
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 10px 20px;
        position: fixed;
        top: 0;
        right: 0;
        left: 0;
        background-color: #333;
        color: white;
    }
    h3{
        margin: 0;
    }
</style>