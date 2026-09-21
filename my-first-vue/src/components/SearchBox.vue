<script setup>
import { ref } from 'vue'

const text = ref('')

const emit = defineEmits(['search'])

function sendSearch() {
  emit('search', text.value)
}
</script>

<template>
  <input
    v-model="text"
    placeholder="جستجو..."
  >

  <button @click="sendSearch">
    جستجو
  </button>
</template>