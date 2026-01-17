

<template>
  <main class="container">
    <HomePage />
    <Timeline />
    <Projects />
    <FooterComponent />
  </main>  
</template>

<script setup>
  import HomePage from './components/HomePage.vue'
  import Timeline from './components/Timeline.vue'
  import Projects from './components/Projects.vue'
  import FooterComponent from './components/Footer.vue'
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
