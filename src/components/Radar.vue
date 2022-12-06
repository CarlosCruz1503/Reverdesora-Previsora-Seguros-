<template>
    <div class="container r-container">
        <div class="r-claves">
            <p class="gray"></p>
            <h1 class="r-h1">Como Funciona?</h1>
        </div>
        <div class="info">
            <div class="row">
                <div class="col-4 info-div">
                    <img src="../../public/img/burbuja1.png" alt="">
                    <p>Presentas el portafolio de iniciativas verdes a desarrollar, eligiendo al menos un proyecto por
                        cada eje (ambiental, social y de gobernanza) y el monto de la inversión.
                    </p>
                </div>
                <div class="col-4 info-div">
                    <img src="../../public/img/burbuja2.png" alt="">
                    <p>Recibes la oferta de coberturas y asistencias que más se ajuste a tus necesidades</p>
                </div>
                <div class="col-4 info-div">
                    <img src="../../public/img/burbuja3.png" alt="">
                    <p>Inicias la implementación de tu portafolio balanceado. Tu decides si deseas asesoría
                        especializada brindada por nuestros aliados y/o líneas de financiación
                    </p>
                </div>
                <div class="col-1"></div>
            </div>
        </div>
        <div class="r-title">
            <h1>QUÉ TAN VERDE QUIERES SER?
            </h1>
        </div>
        <div class="visible">
            <div class="row">
                <div class="col-12 col-xl-2 r-panel">
                    <div class="panel">
                        <h3 id="ambientales">Ambientales</h3>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch1">Gestión Del Agua</label>
                            <input class="form-check-input desactivado" type="checkbox" role="switch" id="switch1"
                                v-on:click="aparecerDesaparecer('#switch1', '#gAgua', 50)">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch2">Economía Circular</label>
                            <input class="form-check-input desactivado" type="checkbox" role="switch" id="switch2"
                                v-on:click="aparecerDesaparecer('#switch2', '#economiaCircular', 500)">

                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch3">Prevención y Control de la contaminación

                            </label>
                            <input class="form-check-input desactivado" type="checkbox" role="switch" id="switch3"
                                v-on:click="aparecerDesaparecer('#switch3', '#pCC', 150)">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch4">Conservación de los ecosistemas y la
                                biodiversidad
                            </label>
                            <input class="form-check-input desactivado" type="checkbox" role="switch" id="switch4"
                                v-on:click="aparecerDesaparecer('#switch4', '#CEB', 500)">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch5">Adaptación al Cambio Climático

                            </label>
                            <input class="form-check-input desactivado" type="checkbox" role="switch" id="switch5"
                                v-on:click="aparecerDesaparecer('#switch5', '#adaptacionCClimatico', 100)">
                        </div>
                    </div>
                    <hr>
                    <div class="panel">
                        <h3 id="sociales">Sociales</h3>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch6">Prevención accidentes
                            </label>
                            <input class="form-check-input desactivado" type="checkbox" role="switch" id="switch6"
                                v-on:click="aparecerDesaparecer('#switch6', '#PC', 20)">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch7">Infraestructura Social
                            </label>
                            <input class="form-check-input desactivado" type="checkbox" role="switch" id="switch7"
                                v-on:click="aparecerDesaparecer('#switch7', '#IS', 200)">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch8">Gestión de Stakeholders y comunidad
                            </label>
                            <input class="form-check-input desactivado " type="checkbox" role="switch" id="switch8"
                                v-on:click="aparecerDesaparecer('#switch8', '#GSC', 30)">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch9">Promoción de empresas y pymes locales
                            </label>
                            <input class="form-check-input desactivado " type="checkbox" role="switch" id="switch9"
                                v-on:click="aparecerDesaparecer('#switch9', '#PEPL', 15)">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch10">Generación de empleo
                            </label>
                            <input class="form-check-input desactivado" type="checkbox" role="switch" id="switch10"
                                v-on:click="(aparecerDesaparecer('#switch10', '#generacionEmpleo', 15))">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch11">Derechos de los trabajadores
                            </label>
                            <input class="form-check-input desactivado" type="checkbox" role="switch" id="switch11"
                                v-on:click="aparecerDesaparecer('#switch11', '#DT', 15)">
                        </div>
                    </div>
                </div>
                <div class="col-12 col-xl-8 d-radar ">
                    <div class='radar'>
                        <div class='sweep'></div>
                    </div>

                    <div class="r-img">
                        <img class="radar-img" src="../../public/img/radar2.png" alt="">
                    </div>
                    <div class="p-radar">
                        <ItemRadar name="gAgua" target="gATarget" targetA="#gATarget" nameLabel="gALabel"
                            Title="Gestión Del Agua" grup="ambiental" Costo="50" cubrimos1="* Amparo por responsabilidad civil por contaminación de fuentes hídricas (Vertimientos)
                            " cubrimo2="* Amparo por gastos de limpieza de fuente hídrica
                            " cubrimos3="* Amparo por gastos para implementar programas de contención ambiental correctivos
                            " cubrimos4="* Amparo por cauciones judiciales en contra del asegurado
                            " noCubrimos1="* Daños ambientales por incumplimiento doloso de normativa ambiental. 
                            " noCubrimos2="* Contaminación de área no inspeccionada previamente
                            " asistencia1="* Asistencia de financiación de programas de gestión ambiental con nuestros aliados (Grupo Bicentenario). 
                            " asistencias2="* Asistencia con Ministerio de Ambiente y entidades involucradas para asesoramiento en implementación de programas de gestión ambiental.
                            " asistencias3="* Asistencia en mantenimiento de equipos de conservación ambiental e infraestructura. 
                            " img="https://cdn-icons-png.flaticon.com/512/999/999049.png
                            " />

                        <ItemRadar name="economiaCircular" target="eCTarget" targetA="#eCTarget" nameLabel="eCLabel"
                            Title="Economia Circular" grup="ambiental" Costo="500" cubrimos1="* Amparo de responsabilidad civil por contaminación de disposición de residuos 
                            " cubrimos2="* Amparo todo riesgo a equipos, maquinaria e infraestructura relacionados con proyectos de implementación de economía circular en cualquier etapa (transporte, implementación y desarrollo)
                            " noCubrimos1="* Daños ambientales por incumplimiento doloso de normativa ambiental. 
                            " noCubrimos2="* Contaminación de área no inspeccionada previamente
                            " noCubrimos3="* Contaminación olfativa derivada de actividades de reciclaje
                            " asistencias1="* Asistencia de financiación de programas de gestión ambiental con nuestros aliados (Grupo Bicentenario). 
                            " asistencias2="* Asistencia con Ministerio de Ambiente y entidades involucradas para asesoramiento en implementación de programas de gestión ambiental.
                            " asistencias3="* Asistencia en mantenimiento de equipos de conservación ambiental e infraestructura. 
                            " img="https://cdn-icons-png.flaticon.com/512/7417/7417583.png
                            " />

                        <ItemRadar name="pCC" target="pCCTarget" targetA="#pCCTarget" nameLabel="pCCLabel" Title=" 
                            Prevención y Control de la contaminación" grup="ambiental" Costo="150" cubrimos1="* Póliza seguro de parque automotor eléctricos, híbridos y/o energía eólica (RC Contractual y Extracontractual, Perdida Severa y menor por Daños / Hurto, gastos de grúa, transporte, y protección de vehículo, así como todo riesgo).
                            " cubrimos2="* Póliza seguro de bicicletas (Perdida severa)
                            " cubrimos3="* Amparo todo riesgo a equipos, maquinaria e infraestructura relacionados con proyectos de implementación de prevención y control de la contaminación en cualquier etapa (transporte, implementación y desarrollo)
                            " noCubrimos1="* Daños ambientales por incumplimiento doloso de normativa ambiental.
                            " asistencias1="* Asistencia de financiación de programas de gestión ambiental con nuestros aliados (Grupo Bicentenario). 
                            " asistencias2="* Asistencia con Ministerio de Ambiente y entidades involucradas para asesoramiento en implementación de programas de gestión ambiental.
                            " asistencias3="* Asistencia en mantenimiento de equipos de conservación ambiental e infraestructura. 
                            " asistencias4="* Asistencia en talleres (pequeños accesorios y llantas estalladas – Vehículo de reemplazo)
                            " img="https://cdn-icons-png.flaticon.com/512/2856/2856787.png
                            " />

                        <ItemRadar name="CEB" target="CEBTarget" targetA="#CEBTarget" nameLabel="CEBLabel" Title="
                                Conservación de los ecosistemas y la biodiversidad" grup="ambiental" Costo="500"
                            cubrimos1="* Póliza de seguro agrícola de inversión por planta para cultivos de tardío rendimiento (Incluye proyectos agroforestales y/o granjas urbanas).
                                " cubrimos2="* Amparo todo riesgo a equipos, maquinaria, insumos e infraestructura relacionados con proyectos de implementación de conservación de los ecosistemas y biodiversidad en cualquier etapa de implementación (transporte, implementación y desarrollo)
                                " noCubrimos1="* Daños ambientales por incumplimiento doloso de normativa ambiental."
                            asistencias1="" />

                        <ItemRadar name="adaptacionCClimatico" target="aCCTarget" targetA="#aCCTarget"
                            nameLabel="aCCLabel" Title="Adaptacion Cambio Climatico" grup="ambiental" Costo="100"
                            Description="Se refiere a cambios en los procesos, prácticas y estructuras para moderar los daños potenciales o para beneficiarse de las oportunidades asociadas con el cambio climático." />



                        <ItemRadar name="PC" target="PCTarget" targetA="#PCTarget" nameLabel="PCLabel" Title="
                            Prevención accidentes" grup="social" Costo="20"
                            Description="Medidas de prevención para los accidentes en el trabajo
                                Colocar de manera correcta los materiales o productos que se procesan en el centro de trabajo. Mantener orden y limpieza en todas las instalaciones, áreas, equipo, maquinaria y herramienta, entre otras." />

                        <ItemRadar name="IS" target="ISTarget" targetA="#ISTarget" nameLabel="ISLabel" Title="
                        Infraestructura Social" grup="ambiental" Costo="200"
                            Description="
                            Los proyectos de infraestructura social son pequeñas obras que tienen como objeto contribuir a satisfacer las necesidades básicas de la población rural en situación de pobreza, y financian las siguientes líneas de intervención: centros educativos, puestos de salud, agua potable, letrinas, trochas, puentes carrozables." />

                        <ItemRadar name="GSC" target="GSCTarget" targetA="#GSCTarget" nameLabel="GSCLabel" Title="
                        Gestión de Stakeholders y comunidad" grup="ambiental" Costo="30"
                            Description="
                            La gestión de relaciones con stakeholders es el proceso a través del cual se fomenta la relación recíproca y beneficiosa entre una empresa y sus grupos de interés (inversores, clientes, proveedores, empleados, medios de comunicación, entre otros)." />


                        <ItemRadar name="PEPL" target="PEPLTarget" targetA="#PEPLTarget" nameLabel="PEPLLabel" Title="
                        Promoción de empresas y pymes locales" grup="ambiental" Costo="15"
                            Description="
                            Son las MIPyMES quienes impulsan el desarrollo económico, generan empleo, especialmente para los jóvenes, y promueven la innovación y el progreso en el sector de las Tecnologías de la Información y las Comunicaciones (TIC)." />

                        <ItemRadar name="generacionEmpleo" target="gETarget" targetA="#gETarget" nameLabel="gELabel"
                            Title="Generación de empleo" grup="social" Costo="15"
                            Description="La generación de empleo es la capacidad que tiene la actividad turística para la creación de nuevos empleos en un destino o centro turístico. Mathienson y Wall (1990) establecen tres tipos de empleos que son generados por la actividad: directos, indirectos e inducidos." />

                        <ItemRadar name="DT" target="DTTarget" targetA="#DTTarget" nameLabel="DTLabel"
                            Title="Derechos de los trabajadores" grup="social" Costo="15" Description="Toda persona tiene derecho al trabajo, a la libre elección de su trabajo, a condiciones equitativas y satisfactorias de trabajo y a la protección contra el desempleo. Toda persona tiene derecho, sin discriminación alguna, a igual salario por trabajo igual.
                            " />
                        <ItemRadar name="antiCorrupcion" target="aCTarget" targetA="#aCTarget" nameLabel="aCLabel"
                            Title="Anti-Corrupcion" grup="gobernanza" Costo="15"
                            Description="El Sistema Nacional Anticorrupción coordina a actores sociales y a autoridades de los distintos órdenes de gobierno, a fin de prevenir, investigar y sancionar la corrupción." />

                        <ItemRadar name="CR" target="CRTarget" targetA="#CRTarget" nameLabel="CRLabel"
                            Title="Confianza y reputación" grup="gobernanza" Costo="20"
                            Description="Es la imagen que proyecta la empresa y la percepción de ésta que tienenus stakeholders (grupos de  sinterés, tanto internos como externos), como resultado del comportamiento desarrollado por la empresa a lo largo del tiempo y de su capacidad para distribuir valor a los mencionados grupos." />
                        <ItemRadar name="TJC" target="TJCTarget" targetA="#TJCTarget" nameLabel="TJCLabel"
                            Title="Trato justo a los clientes" grup="gobernanza" Costo="15"
                            Description="Un buen servicio al cliente no sólo es responder las preguntas del cliente, sino ayudarlo cuando ni siquiera ha pedido nuestra ayuda, adelantarnos a lo que necesita y cubrir sus necesidades de manera eficaz. Existen otros aspectos como la amabilidad, calidad y calidez que también influirán en el servicio ofrecido." />
                        <ItemRadar name="RC" target="RCTarget" targetA="#RCTarget" nameLabel="RCLabel"
                            Title="Rendicion de cuentas" grup="gobernanza" Costo="15"
                            Description="La rendición de cuentas es una oportunidad para que la sociedad evidencie los resultados de la entidad de acuerdo con el cumplimiento de la misión o propósito fundamental, además, de la entrega efectiva de bienes y servicios orientados a satisfacer las necesidades o problemas sociales de sus grupos de valor" />

                        <ItemRadar name="OG" target="OGTarget" targetA="#OGTarget" nameLabel="OGLabel"
                            Title="Órganos de Gobierno" grup="gobernanza" Costo="150"
                            Description="Definición de Órgano de Administración de una empresa

                            Es el equipo de alta dirección (por así llamarlo) y que tendrá la potestad de tomar decisiones de ámbitos diferentes que afecten a la gestión de la empresa" />






                    </div>
                </div>
                <div class="col-12 col-xl-2 r-panel">
                    <div class="panel" id="p-gobernanza">
                        <h3 id="gobernanza">Gobernanza</h3>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch12">Anticorrupción
                            </label>
                            <input class="form-check-input desactivado" type="checkbox" role="switch" id="switch12"
                                v-on:click="aparecerDesaparecer('#switch12', '#antiCorrupcion', 15)">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch13">Confianza y reputación
                            </label>
                            <input class="form-check-input desactivado" type="checkbox" role="switch" id="switch13"
                                v-on:click="aparecerDesaparecer('#switch13', '#CR', 20)">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch14">Trato justo a los clientes
                            </label>
                            <input class="form-check-input desactivado " type="checkbox" role="switch" id="switch14"
                                v-on:click="aparecerDesaparecer('#switch14', '#TJC', 15)">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch15">Rendición de cuentas
                            </label>
                            <input class="form-check-input desactivado " type="checkbox" role="switch" id="switch15"
                                v-on:click="aparecerDesaparecer('#switch15', '#RC', 33)">
                        </div>
                        <div class="form-check form-switch">
                            <label class="form-check-label " for="switch16">Órganos de Gobierno
                            </label>
                            <input class="form-check-input desactivado " type="checkbox" role="switch" id="switch16"
                                v-on:click="aparecerDesaparecer('#switch16', '#OG', 150)">
                        </div>
                        <label class="form-label" for="">Inversion
                        </label>
                        <input type="text" class="form-control" id="inversion" value="0">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import ItemRadar from './ItemRadar.vue'
export default {
    name: 'Radar',
    components: {
        ItemRadar,
    },
    mounted() {
        let switches = document.querySelectorAll(".form-check-input");
        let modal = document.querySelectorAll(".modal");
        let boton = document.querySelectorAll(".btn-close");
        let boton2 = document.querySelectorAll(".close-gray");
        for (let i = 0; i < 16; i++) {
            switches[i].addEventListener("click", (e) => {
                if (switches[i].classList[1] == 'activado') {
                    if (window.innerWidth < 768) {
                        modal[i + 1].classList.add("show")
                        modal[i + 1].setAttribute("aria-modal", "true")
                        modal[i + 1].setAttribute("role", "dialog")
                        modal[i + 1].setAttribute("aria-hidden", "")
                        modal[i + 1].setAttribute("aria-labelledby", "gALabel")
                        modal[i + 1].style.display = "block"
                    }
                }
            })
            boton[i].addEventListener("click", (e) => {
                if (window.innerWidth < 768) {
                    modal[i + 1].classList.remove("show")
                    modal[i + 1].setAttribute("aria-modal", "")
                    modal[i + 1].setAttribute("role", "switch")
                    modal[i + 1].setAttribute("aria-hidden", "true")
                    modal[i + 1].setAttribute("aria-labelledby", "")
                    modal[i + 1].style.display = "none"
                }
            })
            boton2[i].addEventListener("click", (e) => {
                if (window.innerWidth < 768) {
                    modal[i + 1].classList.remove("show")
                    modal[i + 1].setAttribute("aria-modal", "")
                    modal[i + 1].setAttribute("role", "switch")
                    modal[i + 1].setAttribute("aria-hidden", "true")
                    modal[i + 1].setAttribute("aria-labelledby", "")
                    modal[i + 1].style.display = "none"

                }
            })
        }

    },
    methods: {
        aparecerDesaparecer(switchNum, idButton, costo,) {
            let switchX = document.querySelector(switchNum);
            let item = document.querySelector(idButton);
            let inversion = document.querySelector("#inversion");
            if (switchX.classList[1] == 'desactivado') {
                switchX.classList.remove("desactivado")
                switchX.classList.add("activado")
                item.classList.remove("Quitar")
                inversion.value = parseInt(inversion.value) + costo
            } else {
                switchX.classList.remove("activado")
                switchX.classList.add("desactivado")
                item.classList.add("Quitar")
                inversion.value = parseInt(inversion.value) - costo
            }
        }

    }
}


</script>

