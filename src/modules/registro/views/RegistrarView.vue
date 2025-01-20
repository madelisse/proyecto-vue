<template>
 <div>
  <h2>Formulario de registro</h2>
  <Form :validation-schema="schema" @submit="">
   <div class="form">
    <label for="name">Nombre:</label>
    <Field type="text" name="name" id="name" placeholder="ingrese su npombre" />
    <ErrorMessage name="name"></ErrorMessage>
   </div>
   <div class="form">
    <label for="email">E-mail:</label>
    <Field type="email" name="email" id="email" placeholder="ingrese su email" />
    <ErrorMessage name="email"></ErrorMessage>
   </div>
   <div class="form">
    <button type="submit">Registrar</button>
   </div>
  </Form>
 </div>
</template>

<script setup>
import { Form, Field, ErrorMessage } from 'vee-validate';
import { schema } from '../schemas/ValidationSchema';

const onSubmit = () => {
 console.log('se ah enviado el formulario');
}
</script>

<style scoped>
.form {
 margin-bottom: 10px;
}
</style>