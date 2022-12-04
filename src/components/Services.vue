<template>
    <div class="container">
        <div class="d-services">
            <p class="gray">¿ POR QUÉ ?</p>
            <h1 class="s-h1">Tú y tu empresa merecen este seguro</h1>
            <div class="row r-services">
                <div class="col-12 col-md-6 col-lg-4 r-services">
                    <ServicesCard icon="bi bi-people-fill" SText="Optimización de su responsabilidad social empresarial."
                        SButton="Ver ventajas de ser una empresa ASG" SNumber="1"
                        link="https://redshift.autodesk.es/que-es-asg/" />
                </div>
                <div class="col-12 col-md-6 col-lg-4 r-services">
                    <ServicesCard icon="bi bi-cash"
                        SText="Una empresa ambientalmente responsable debe pagar menos impuestos"
                        SButton="Legislaciones sobre sostenibilidad empresarial" SNumber="2"
                        link="https://www.minambiente.gov.co/lideres-ambientales/normativa-ambiental/" />
                </div>
                <div class="col-12 col-md-6 col-lg-4 r-services">
                    <ServicesCard icon="bi bi-piggy-bank"
                        SText="Aseguraremos su inversion, así que puede desarollar el proyecto con tranquilidad "
                        SButton="Calculadora de costos a ahorrar" SNumber="3" link="https://www.soyeficiente.com/" />
                </div>
            </div>
            <div class="row r-services">
                <div class="col-12 col-md-6 col-lg-4 r-services">
                    <ServicesCard icon="bi bi-bank"
                        SText="Al ser una empresa sostenible y responsable ambientalmente podría obtener beneficios gubernamentales"
                        SButton="Legislaciones sobre sostenibilidad empresarial" SNumber="4"
                        link="https://www.minambiente.gov.co/lideres-ambientales/normativa-ambiental/" />
                </div>
                <div class="col-12 col-md-6 col-lg-4 r-services">
                    <ServicesCard icon="bi bi-lightning"
                        SText="Su empresa optimizara y gastará menos energía, con lo cual podra destinar el dinero ahorrado en otro lugar"
                        SButton="Info sobre proyecto para generación de energía solar" SNumber="5"
                        link="https://becquel.com/blog/es/proceso-cambio-energia-solar/" />
                </div>
                <div class="col-12 col-md-6 col-lg-4 r-services">
                    <ServicesCard icon="bi bi-person-heart"
                        SText="Cumplir con criterios ASG, hará que su empresa sea percibida de mejor manera por los clientes"
                        SButton="
                        Ver ventajas de ser una empresa ASG" SNumber="6"
                        link="https://redshift.autodesk.es/que-es-asg/" />
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import ServicesCard from './Services-card.vue';
export default {
    name: 'Services',
    components: {
        ServicesCard,
    }
}

</script>