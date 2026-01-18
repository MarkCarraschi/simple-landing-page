<template>
    <footer class="bg-dark text-light py-3 footer-snap">
        <div class="container text-center">
            <div class="mb-3">                
                <div class="d-flex justify-content-center gap-4"> 
                    <a 
                        v-for="url in listSocialMedia"
                        :key="url?.Id"
                        :href="url.Url" 
                        target="_blank" 
                        class="btn btn-outline-light">
                            <i :class="url.StyleClass" aria-hidden="true"></i>
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
    const listSocialMedia = [
        {
            "Id": 0,            
            "Url": "https://www.linkedin.com/in/marcus-carraschi",
            "StyleClass": "bi bi-linkedin fs-4"
        },
        {
            "Id": 1,            
            "Url": "https://github.com/MarkCarraschi",
            "StyleClass": "bi bi-github fs-4"
        },
        {
            "Id": 2,            
            "Url": "marcuscarraschy@gmail.com",
            "StyleClass": "bi bi-envelope fs-4"
        }
    ]
</script>

<style scoped>
.footer-snap {
    scroll-snap-align: end;
}
</style>