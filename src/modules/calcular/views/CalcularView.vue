<template>
  <h3>Propiedades computadas</h3>
  <input type="text" v-model="valor">
  {{ valorCalculado }}
</template>
<script setup>
  import {ref, computed} from 'vue';
  const valor = ref('');
  const valorCalculado = computed(()=>{
    return valor.value * 3;
  })
</script>
<style scoped>
</style>
