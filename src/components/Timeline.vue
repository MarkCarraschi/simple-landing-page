<template>
    <section class="timeline-section my-5">
        <h2 class="text-center mb-5 fw-bold">{{ titlePagePortuguese }}</h2>
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div v-for="item in listExperiencePortuguese" :key="item.Id" class="card mb-4 border-0 shadow-sm">
                    <div :class="item?.StyleClass">
                        <h4 class="card-title fw-bold">{{ item?.Role }}</h4>
                        <h5 class="card-title fw-bold">{{ item?.CompanyName }}</h5>
                        <h6 class="text-muted mb-2">{{ item?.Range }}</h6>
                        <p class="card-text">
                            {{ item?.Description }}
                        </p>
                    </div>
                </div>                
            </div>
        </div>
    </section>
</template>>

<script setup>

const titlePagePortuguese = "Experiência profissional";

const listExperiencePortuguese = [
    {
        "Id": 0,
        "Role": "Desenvolvedor Full Stack [Pl.]",
        "Description" : "Atuação em P&D no setor de varejo digital, liderando frentes Full Stack (C#/.NET, Vue.js) e Mobile Híbrido. " + 
            "\nResponsável pela arquitetura e desenvolvimento de APIs REST, componentes de ERP e unificação de ecossistemas de pagamento (POS/Web), garantindo qualidade de código (SonarQube) e entregas em ambiente Agile/Azure DevOps.",
        "CompanyName" : "Linx - Stone Co",
        "Range": "NOV/2021 - Atualmente",
        "StyleClass": "card-body border-start border-4 border-success ps-4"
    },
    {
        "Id": 1,
        "Role": "Desenvolvedor Full Stack [Jr.]",
        "Description" : "Atuação end-to-end em soluções corporativas, desenvolvendo desde portais de inspeção de código (Python/Jenkins) e integrações JIRA/SAP, até sistemas de gestão documental em .NET MVC e SQL Server.\n"
        + "Responsável também pela gestão de configuração (GitLab) e deploy em projetos de tráfego aéreo.",
        "CompanyName" : "Atech S.A. - Embraer Group",
        "Range": "NOV/2019 - OUT/2021",
        "StyleClass": "card-body border-start border-4 border-secondary ps-4"

    },
    {
        "Id": 2,
        "Role": "Analista de Sistemas [Jr.]",
        "Description": "Atuação full stack na evolução de sistemas (.NET, SQL Server, Bootstrap) e implementação de solução PWA para portabilidade mobile de CRM.",        
        "CompanyName" : "Matrix Saúde",
        "Range": "MAI/2019 - NOV/2019",
        "StyleClass": "card-body border-start border-4 border-secondary ps-4"
    }
];

//TODO
/*const listExperienceEnglish = [
    {}
];*/

</script>