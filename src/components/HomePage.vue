<template>
    <section class=".hero d-flex flex-column align-items-center justify-content-center text-center py-5">
        <h1 class="display-4 fw-bold">Marcus Vinicius Nobre Carraschi</h1>
        <p class="lead text-muted">Desenvolvedor Full Stack [.NET/Vue]</p>
        <div class="d-flex gap-3 mt-4">
            <a :href="urlLinkedIn" class="btn btn-dark btn-lg px-5">LinkeDin</a>
            <a :href="urlGitHub" class="btn btn-outline-dark btn-lg px-5">GitHub</a>            
        </div>        
    </section>
</template>

<style scoped>
    .hero {
        padding: 4rem 1rem;
        text-align: center;
    }
</style>

<script setup>
    const urlLinkedIn = "https://www.linkedin.com/in/marcus-carraschi";
    const urlGitHub = "https://github.com/MarkCarraschi";
</script>