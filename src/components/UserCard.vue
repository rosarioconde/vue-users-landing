<template>  
  <div class="user-card p-4 bg-gray-100 rounded">
    <h3>{{ user.name }}</h3>
    <p>{{ user.email }}</p>
  </div>
</template>

<script setup>
defineProps({
  user: Object
})
</script>