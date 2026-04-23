<script setup>
import { ref } from 'vue'
import viteLogo from '../assets/vite.svg'
import heroImg from '../assets/hero.png'
import vueLogo from '../assets/vue.svg'
import Card from './Card.vue'
import Footer from './footer.vue'

const count = ref(0)
</script>

<template>
  <section id="center">
    <div>
      <h1>Vue</h1>
    </div>
    <button type="button" class="counter" @click="count++">
      Count is {{ count }}
    </button>

    <Card />
  </section>
  <Footer />
</template>
