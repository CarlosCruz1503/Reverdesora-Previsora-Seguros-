<template>
    <div class="container con-clave">
        <div class="d-claves">
            <p class="gray">BENEFICIOS</p>
            <h1 class="c-h1">Lo que te ofrecemos</h1>
        </div>
        <div class="row">
            <div class="col-12 col-lg-6 c-img">
                <img src="../../public/img/5250872-1080x675.jpg" alt="">
            </div>
            <div class="col-12 col-lg-6 c-claves">
                <CardClave title="1. Bonos" text="El valor de las primas serán invertidas en bonos verdes que serán destinados a sus propios proyectos que generen impacto positivo en el medio ambiente
                " icon="bi bi-tree"/>
                <CardClave title="2. Ajustable" text="Tanto las coberturas como las asistencias se acomodan a las iniciativas propuestas, el valor de la prima considera el valor del portafolio completo para aplicar tasas preferenciales.
                " icon="bi bi-rocket-takeoff"/>
                <CardClave title="3. Asesoría
                " text="Acceso al directorio de aliados que pueden acompañarlo en la materialización de las iniciativas mapeadas.
                " icon="bi bi-map"/>
                <CardClave title="4. Desempeño
                " text="Acceso a herramientas para la medición de los indicadores de desempeño en la gestión de los riesgos.
                " icon="bi bi-file-earmark-bar-graph"/>
            </div>
        </div>
    </div>
</template>

<script>
import CardClave from './Card-Clave.vue'
export default {
    name: 'Claves',
    components: {
        CardClave,
    }
}
</script>