<script setup>
import { ref } from 'vue'

const color = ref( 'pink' )
color.value = 'green'

</script>

<template>
  <h1>Hola Vue 3.2</h1>
  <h3>{{ color }}</h3>
  <button @click="color = 'pink'">pink</button>
  <button @click="color = 'indigo'">indigo</button>
  <button @click="color = 'green'">green</button>
</template>


<style scoped>
h1 {
  color: v-bind( color );
}
</style>