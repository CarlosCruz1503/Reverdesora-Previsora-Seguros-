<template>
    <div class="container">
        <div class="f-claves">
            <p class="gray">RESOLVEMOS TUS DUDAS</p>
            <h1 class="f-h1">Preguntas frecuentes</h1>
        </div>
        <div class="faq">
            <div class="row">
                <div class="col-12 col-md-2"></div>
                <div class="col-12 col-md-8">
                    <div class="accordion" id="accordionExample">
                        <FaqQ name="pregunta" nameNumber="pregunta1" ANameNumber="#pregunta1"
                            FaqT="¿Qué es reverdesora?" Answer="Reverdesora es un paquete de seguros ajustado a las necesidades de los clientes y en línea con las iniciativas que conforman cada portafolio de iniciativas ASG.
                        " />
                        <FaqQ name="preguntaa" nameNumber="pregunta2" ANameNumber="#pregunta2"
                            FaqT="¿Qué pasá si invierto y de repente suben los precios de generación de energía renovable?"
                            Answer="La previsora te asegura tus fondos y que con la inversión inicial tu proyecto se finalice, Previsora responde.. Tú tranquilo!!!  " />
                        <FaqQ name="preguntaaa" nameNumber="pregunta3" ANameNumber="#pregunta3"
                            FaqT="¿Hacia quiénes va dirigido este seguro?"
                            Answer="Empresas que cumplan con los criterios de elegibilidad de la taxonomía verde" />
                        <FaqQ name="preguntaaaa" nameNumber="pregunta4" ANameNumber="#pregunta4"
                            FaqT="¿Por qué existe este seguro?" Answer="“Reverdesora”, es el primer seguro verde en Colombia y en el mundo creado para proteger a las organizaciones que cumplen con los criterios de elegibilidad de la taxonomía verde, durante la implementación de sus portafolios de iniciativas ASG orientadas a reducir el riesgo de sostenibilidad es decir, aquellos riesgos que por circunstancias ambientales, sociales o de gobernanza, produzcan un impacto adverso al desarrollo económico ambientalmente sostenible.
                            " />
                        <FaqQ name="preguntaaaaa" nameNumber="pregunta5" ANameNumber="#pregunta5"
                            FaqT="¿Qué cubre este seguro?" Answer="Ejemplo de coberturas:
                            Responsabilidad Civil por contaminación de predios, 
                            Seriedad de oferta, 
                            Buen manejo y correcta inversión del anticipo, 
                            Cumplimiento, 
                            Pago de salarios, 
                            Estabilidad de obra, entre muchos otros 
                            
                            " />
                        <FaqQ name="preguntaaaaaa" nameNumber="pregunta6" ANameNumber="#pregunta6"
                            FaqT="¿Comó se calcula la prima?"
                            Answer="El portafolio ASG es valorizado y partir del alcance definido para cada una de las iniciativas y horizontes, se estimará el paquete de coberturas adecuado y así mismo el valor de la prima a pagar." />
                    </div>
                    <div class="col-12 col-md-2"></div>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
import FaqQ from './Faq-W.vue'
export default {
    name: 'Faq',
    components: {
        FaqQ,
    }
}

</script>