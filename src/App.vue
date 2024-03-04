<script setup>
import { ref } from 'vue'

const contador = ref(0)

const contador2 = ref(0);

function decrementar() {
  contador.value--
 
}

function encrementar() {
  contador.value++
}

function decrementar2(){
    contador2.value--
}

function encrementar2(){
    contador2.value++
}

</script>
<template>
    <div class="contador "><h1>Contador</h1>
      <button @click="encrementar">+</button>
      <button @click="decrementar">-</button>
      <p>O valor do contador é: {{ contador }}</p>
    </div>
    <div class="contador 2" ><h1>Contador2</h1>
      <button @click="encrementar2">+</button>
      <button @click="decrementar2">-</button>
      <p>O valor do contador é: {{ Contador2 }}</p></div>

      <div>
        <p v></p>

      </div>
</template>