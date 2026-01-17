<template>
    <section class="projects-section py-5 bg-light">
        <div class="container">
            <h2 class="text-center mb-5 fw-bold"> Projetos</h2>
            <div class="row">
                <div v-for="project in projects" :key="project.title" class="col-md-4 mb-4">
                    <div class="card-body">
                        <h5 class="card-title fw-bold">{{ project.title }}</h5>
                        <p class="card-text text-muted">{{ project.description }}</p>
                    </div>
                    <div class="card-footer bg-white border-0 pb-3">
                        <a :href="project.link" class="btn btn-outline-primary btn-sm w-100">Fonte</a>
                    </div>
                </div>
            </div>
        </div>

    </section>
</template>

<script setup>
    const projects = [        
        {
            title: "WebApi C# - .NET8",
            description: "Backend robusto usando Docker, Service Layer e SOLID",
            link: '#'
        },
        {
            title: "Refatoração de PDV",
            description: "Sol. feita em conjunto com o intuito de refatorar um código legado",
            link: '#'
        },
        {
            title: "Landing Page Vue",
            description: "Um portifólio pessoal construído em Vue 3 e Bootstrap",
            link: '#'
        },
        
        {
            title: "Landing Page Vue",
            description: "Um portifólio pessoal construído em Vue 3 e Bootstrap",
            link: '#'
        },
        {
            title: "WebApi C# - .NET8",
            description: "Backend robusto usando Docker, Service Layer e SOLID",
            link: '#'
        },
        {
            title: "Refatoração de PDV",
            description: "Sol. feita em conjunto com o intuito de refatorar um código legado",
            link: '#'
        },
    ]
</script>