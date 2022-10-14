<template>
  <div class="bg-green-500 text-red-500">
    <h1>One</h1>
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