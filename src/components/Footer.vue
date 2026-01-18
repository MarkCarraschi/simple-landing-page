<template>
    <footer class="bg-dark text-light py-3 footer-snap">
        <div class="container text-center">
            <div class="mb-3">                
                <div class="d-flex justify-content-center gap-4">
                    <a :href="urlLinkedIn" target="_blank" class="btn btn-outline-light">
                        <i class="bi bi-linkedin fs-4" aria-hidden="true"></i>
                    </a>
                    <a :href="urlGitHub" target="_blank" class="btn btn-outline-light">
                        <i class="bi bi-github fs-4" aria-hidden="true"></i>
                    </a>
                    <a :href="`mailto:${urlEmail}`" class="btn btn-outline-light">
                        <i class="bi bi-envelope fs-4" aria-hidden="true"></i>
                    </a>
                </div>
            </div>
            <hr class="border-secondary w-50 mx-auto opacity-25" />
            <p class="m-0 text-secondary small mt-4">
                &copy; {{ new Date().getFullYear() }} Marcus V. N. Carraschi
            </p>
        </div>
    </footer>
</template>

<script setup>
    const urlLinkedIn = "https://www.linkedin.com/in/marcus-carraschi";
    const urlGitHub = "https://github.com/MarkCarraschi";
    const urlEmail = "marcuscarraschy@gmail.com"
</script>

<style scoped>
.footer-snap {
    scroll-snap-align: end;
}
</style>