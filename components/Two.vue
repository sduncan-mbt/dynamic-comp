<template>
  <div class="bg-red-500 text-green-500">
    <h1>Two</h1>
    <h1>{{ values.title }}</h1>
    <p>Id {{ values.id }}</p>
    <p>Name {{ values.name }}</p>
  </div>
</template>

<script setup>
const props = defineProps({
  values: Object
})
</script>