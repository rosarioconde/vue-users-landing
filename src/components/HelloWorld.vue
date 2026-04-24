<script setup>
import { ref } from 'vue'
import viteLogo from '../assets/vite.svg'
import heroImg from '../assets/hero.png'
import vueLogo from '../assets/vue.svg'
import Card from './Card.vue'
import Footer from './footer.vue'
import Cards from './List.vue'
import List from './List.vue'

const count = ref(0)
</script>

<template>
  <section id="center">
    <div>
      <h1>Vue</h1>
    </div>
    <Card />
    <List />
  </section>
  <Footer />
</template>
