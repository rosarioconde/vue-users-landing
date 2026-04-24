<template>
  <UserCard
    v-for="user in users"
    :key="user.id"
    :user="user"
  />
</template>

<script setup>
import UserCard from './UserCard.vue' //componente hijo

import {
  ref,
  onMounted
} from 'vue'


const users = ref([])

onMounted(async () => {
  const res = await fetch('https://jsonplaceholder.typicode.com/users')
  users.value = await res.json()
})
</script>
