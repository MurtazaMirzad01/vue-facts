<script setup>
import {ref} from 'vue';
const facts = ref([
    {
        adjective: "I'm Lightweight",
        description: "I am incredibly small and fast! My core library is only around 30KB, so I won't slow you down."
    },
    {
        adjective: "I'm Approachable",
        description: "Easy to learn and use, even for beginners. I have a gentle learning curve, clear documentation, and a supportive community."
    },
    {
        adjective: "I'm Versatile",
        description: "I can handle everything from simple interactive elements to complex single-page applications. I'm great for small projects and large-scale applications alike."
    }

]);
</script>

<template>
    <main>
        <section v-for ="i in facts" :key="i">
            <h2>{{i.adjective}}</h2>
            <p>{{i.description}}</p>
        </section>
    </main>
</template>

<style scoped>
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