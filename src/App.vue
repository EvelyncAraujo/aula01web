<script setup>
import { ref } from "vue";
const name = ref(`Evelyn linda`)
const idade = ref(15);
const bio = ref(``);
</script>

<template>
  <h1> Aula 04 interligação em formulários</h1>
  <br>
  <div>
    <label>Nome:</label>
    <input type="text" v-model="name" />

    <p>Nome: {{ name }}</p>
    <button @click="name = ``">Limpar</button>
  </div>
  <br>
  <div>
    <label>idade:</label>
    <input type="number" v-model="idade" />
    <button @click="idade = ``">Limpar</button>
  </div>
  <br>
  <div> 
    <label for="sexo">Informe seu sexo </label>
    <input type="radio" v-model="sexo" value="masculino" /> Masculino
    <input type="radio" v-model="sexo" value="feminino" /> Feminino
  </div>
<br>
<div>
   <label>Sua bio:</label>
    <input type="text" v-model="bio" />
    <button @click="bio = ``">Limpar</button>
  </div>



</template>

<style>
h1{
  text-align: center;
  font-size: 20px;
  
}
</style>
