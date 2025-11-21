<script setup>
import { ref } from 'vue';
const facts = ref([
  {
    highlight: 'Lightweight',
    text: 'I am incredibly small and fast! My core library is only around 30KB, so I won\'t slow you down.',
  },
  {
    highlight: 'Approachable',
    text: 'Easy to learn and use, even for beginners. I have a gentle learning curve, clear documentation, and a supportive community.'
  },
  {
    highlight: 'Versatile',
    text: 'I can handle everything from simple interactive elements to complex single-page applications. I\'m great for small projects and large-scale applications alike.',
  }
  
])
</script>

<template>
  <main>
    <section v-for="fact in facts">
      <h2>
        I'm <span class="highlight">{{fact.highlight}}</span>
      </h2>
      <p>
        {{fact.text}}
      </p>
    </section>
    
    
  </main>
</template>

<style scoped>
/* MAIN CSS */
main {
  margin-top: 15px;
}

section {
  margin-top: 25px;
}

h2 {
  font-size: 1.3rem;
  color: #34495e;
  margin-bottom: 3px;
}

p {
  font-size: 0.9rem;
  color: #555;
}

/**********/
</style>