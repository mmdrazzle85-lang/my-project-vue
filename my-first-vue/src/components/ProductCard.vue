<script setup>
const props = defineProps(['product'])

const emit = defineEmits(['addToCart'])

function addProduct() {
  emit('addToCart', props.product)
}
</script>

<template>
  <div>
    <h2>{{ props.product.name }}</h2>

    <p>قیمت: {{ props.product.price }}</p>

    <button @click="addProduct">
      افزودن به سبد
    </button>
  </div>
</template>