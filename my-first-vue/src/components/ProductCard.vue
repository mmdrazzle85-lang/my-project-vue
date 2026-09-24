<!-- <script setup>

defineProps(['product'])

</script>

<template>

  <div>
    <h2>{{ product.name }}</h2>

    <p>قیمت: {{ product.price }} تومان</p>

    <p>دسته‌بندی: {{ product.category }}</p>
    <p>موجودی{{ product.mojodi }}</p>
  </div>

</template> -->








<script setup>

const props = defineProps(['product'])

const emit = defineEmits(['addToCart'])

function addProduct() {
  emit('addToCart', props.product)
}

</script>

<template>

  <div>
    <h2>{{ product.name }}</h2>

    <p>قیمت: {{ product.price }} تومان</p>

    <p>دسته‌بندی: {{ product.category }}</p>

    <button @click="addProduct">
      افزودن به سبد
    </button>
  </div>

</template>