

<template>
  <main class="container">
    <Hero />
    <Timeline />
  </main>
  
</template>

<script setup>
  import Hero from './components/Hero.vue'
  import Timeline from './components/Timeline.vue'

</script>

<style scoped>
/* 1. O container principal (a página toda) */
html {
  scroll-snap-type: y mandatory; /* Ativa o ímã no eixo Y (vertical) */
  scroll-behavior: smooth;       /* Deixa o movimento suave */
}

/* 2. As "lâminas" do slide (nossas seções) */
section {
  /* Ocupa no MÍNIMO 100% da altura da tela */
  min-height: 100vh;
  
  /* Alinha o topo da seção com o topo da tela ao soltar o scroll */
  scroll-snap-align: start;

  /* Centraliza o conteúdo verticalmente (opcional, mas fica bonito) */
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>
