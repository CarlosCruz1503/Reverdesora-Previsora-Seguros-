<template>
    <div class="container r-container">
        <div class="r-claves">
            <p class="gray">RADAR DE PROYECTOS</p>
            <h1 class="r-h1">Radar</h1>
        </div>
        <div class="visible">
            <div class="row">
                <div class="col-12 col-lg-9 d-radar ">
                    <div class='radar'>
                        <div class='sweep'></div>
                    </div>
                    <div class="r-img">
                        <img class="radar-img" src="../../public/img/radar2.png" alt="">
                    </div>
                    <div class="p-radar">
                        <ItemRadar name="economiaCircular" target="eCTarget" targetA="#eCTarget" nameLabel="eCLabel"
                            Title="Economia Circular" grup="ambiental"
                            Description="La economía circular establece un modelo de producción y consumo más sostenible, en el que las materias primas se mantienen más tiempo en los ciclos productivos y pueden aprovecharse de forma recurrente, procurando con ello generar muchos menos residuos." />
                        <ItemRadar name="antiCorrupcion" target="aCTarget" targetA="#aCTarget" nameLabel="aCLabel"
                            Title="Anti-Corrupcion" grup="gobernanza"
                            Description="El Sistema Nacional Anticorrupción coordina a actores sociales y a autoridades de los distintos órdenes de gobierno, a fin de prevenir, investigar y sancionar la corrupción." />
                        <ItemRadar name="generacionEmpleo" target="gETarget" targetA="#gETarget" nameLabel="gELabel"
                            Title="Generación de empleo" grup="social"
                            Description="La generación de empleo es la capacidad que tiene la actividad turística para la creación de nuevos empleos en un destino o centro turístico. Mathienson y Wall (1990) establecen tres tipos de empleos que son generados por la actividad: directos, indirectos e inducidos." />
                        <ItemRadar name="adaptacionCClimatico" target="aCCTarget" targetA="#aCCTarget"
                            nameLabel="aCCLabel" Title="Adaptacion Cambio Climatico" grup="ambiental"
                            Description="Se refiere a cambios en los procesos, prácticas y estructuras para moderar los daños potenciales o para beneficiarse de las oportunidades asociadas con el cambio climático." />
                        <ItemRadar name="trabajoRemoto" target="rWTarget" targetA="#rWTarget" nameLabel="rWLabel"
                            Title="Trabajo remoto" grup="social"
                            Description="El trabajo remoto describe un entorno profesional en el que los empleados pueden trabajar desde casa o desde cualquier otro lugar fuera de la oficina física de su empresa. A menudo, implica crear un espacio de trabajo en casa." />
                        <ItemRadar name="diversidad" target="dTarget" targetA="#dTarget" nameLabel="dLabel" Title="
                            Diversidad, Equidad, Inclusión, Pertenencia" grup="social"
                            Description="La tendencia de Diversidad, Equidad, Inclusión, Pertenencia, también conocida como 'DEIB', se refiere a cuatro conceptos que trabajan en conjunto para reforzar la responsabilidad social dentro de las organizaciones, lo que resulta en un aumento de la eficacia, productividad, dinámica y creatividad de una organización al tiempo que garantiza las personas tienen las mismas oportunidades y se sienten valoradas." />
                        <ItemRadar name="energiaAlternativa" target="sEATarget" targetA="#sEATarget"
                            nameLabel="sEALabel" Title=" 
                            Soluciones de energía alternativa" grup="ambiental"
                            Description="
                            La tendencia de Soluciones de Energía Alternativa abarca la variedad de tecnologías e infraestructura relacionada que aprovechan, almacenan y usan energía de fuentes renovables e inagotables." />
                        <ItemRadar name="descarbonizacion" target="decTarget" targetA="#decTarget" nameLabel="decLabel"
                            Title="
                            Descarbonización" grup="ambiental"
                            Description="
                            La tendencia de la descarbonización es el movimiento hacia la reducción de la cantidad de dióxido de carbono (CO2) y equivalentes de dióxido de carbono (CO2e) en la atmósfera." />
                    </div>
                </div>
                <div class="col-12 col-lg-3 r-panel">
                    <div class="panel">
                        <div class="form-check form-switch">
                            <input class="form-check-input desactivado" v-on:click="Ambientales()" type="checkbox"
                                role="switch" id="switch1">
                            <label class="form-check-label " for="switch1">Ambientales</label>
                        </div>
                        <div class="form-check form-switch">
                            <input class="form-check-input desactivado" v-on:click="Sociales()" type="checkbox"
                                role="switch" id="switch2">
                            <label class="form-check-label " for="switch2">Sociales</label>
                        </div>
                        <div class="form-check form-switch">
                            <input class="form-check-input desactivado " v-on:click="Gobernanzas()" type="checkbox"
                                role="switch" id="switch3">
                            <label class="form-check-label " for="switch3">Gobernanza</label>
                        </div>
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
    methods: {
        Ambientales() {
            let items = document.querySelectorAll(".radar-item");
            let switch1 = document.querySelector("#switch1");
            let switch2 = document.querySelector("#switch2");
            let switch3 = document.querySelector("#switch3");

            if (switch1.classList[1] == 'desactivado') {
                switch1.classList.remove("desactivado")
                switch1.classList.add("activado")
                for (const value of items.values()) {
                    value.classList.add("Quitar")
                    if (value.classList[1] == 'ambiental') {
                        console.log(value)
                        value.classList.remove("Quitar")
                    } else if (switch2.classList[1] == 'activado') {
                        if (value.classList[1] == 'social') {
                            console.log(value)
                            value.classList.remove("Quitar")
                        } else {
                            value.classList.add("Quitar")
                        }
                    } else if (switch3.classList[1] == 'activado') {
                        if (value.classList[1] == 'gobernanza') {
                            console.log(value)
                            value.classList.remove("Quitar")
                        } else {
                            value.classList.add("Quitar")
                        }
                    }

                }
            } else {
                switch1.classList.remove("activado")
                switch1.classList.add("desactivado")
                if (switch2.classList[1] == 'desactivado' && switch3.classList[1] == 'desactivado') {
                    for (const value of items.values()) {
                        value.classList.remove("Quitar")
                    }
                }
            }
            if (switch1.classList[1] == 'desactivado' && (switch2.classList[1] == 'activado' || switch3.classList[1] == 'activado')) {
                for (const value of items.values()) {
                    if (value.classList[1] == 'ambiental') {
                        value.classList.add("Quitar")
                    }
                }
                switch1.classList.remove("activado")
                switch1.classList.add("desactivado")
            }
        },
        Sociales() {
            let items = document.querySelectorAll(".radar-item");
            let switch1 = document.querySelector("#switch1");
            let switch2 = document.querySelector("#switch2");
            let switch3 = document.querySelector("#switch3");

            if (switch2.classList[1] == 'desactivado') {
                switch2.classList.remove("desactivado")
                switch2.classList.add("activado")
                for (const value of items.values()) {
                    value.classList.add("Quitar")
                    if (value.classList[1] == 'social') {
                        console.log(value)
                        value.classList.remove("Quitar")
                    } else if (switch1.classList[1] == 'activado') {
                        if (value.classList[1] == 'ambiental') {
                            console.log(value)
                            value.classList.remove("Quitar")
                        } else {
                            value.classList.add("Quitar")
                        }
                    } else if (switch3.classList[1] == 'activado') {
                        if (value.classList[1] == 'gobernanza') {
                            console.log(value)
                            value.classList.remove("Quitar")
                        } else {
                            value.classList.add("Quitar")
                        }
                    }

                }
            } else {
                switch2.classList.remove("activado")
                switch2.classList.add("desactivado")
                if (switch1.classList[1] == 'desactivado' && switch3.classList[1] == 'desactivado') {
                    for (const value of items.values()) {
                        value.classList.remove("Quitar")
                    }
                }
            }
            if (switch2.classList[1] == 'desactivado' && (switch1.classList[1] == 'activado' || switch3.classList[1] == 'activado')) {
                for (const value of items.values()) {
                    if (value.classList[1] == 'social') {
                        value.classList.add("Quitar")
                        console.log("hola")
                    }
                }
                switch2.classList.remove("activado")
                switch2.classList.add("desactivado")
            }
        },
        Gobernanzas() {
            let items = document.querySelectorAll(".radar-item");
            let switch1 = document.querySelector("#switch1");
            let switch2 = document.querySelector("#switch2");
            let switch3 = document.querySelector("#switch3");

            if (switch3.classList[1] == 'desactivado') {
                switch3.classList.remove("desactivado")
                switch3.classList.add("activado")
                for (const value of items.values()) {
                    value.classList.add("Quitar")
                    if (value.classList[1] == 'gobernanza') {
                        console.log(value)
                        value.classList.remove("Quitar")
                    } else if (switch1.classList[1] == 'activado') {
                        if (value.classList[1] == 'ambiental') {
                            console.log(value)
                            value.classList.remove("Quitar")
                        } else {
                            value.classList.add("Quitar")
                        }
                    } else if (switch2.classList[1] == 'activado') {
                        if (value.classList[1] == 'social') {
                            console.log(value)
                            value.classList.remove("Quitar")
                        } else {
                            value.classList.add("Quitar")
                        }
                    }

                }
            } else {
                switch3.classList.remove("activado")
                switch3.classList.add("desactivado")
                if (switch1.classList[1] == 'desactivado' && switch2.classList[1] == 'desactivado') {
                    for (const value of items.values()) {
                        value.classList.remove("Quitar")
                    }
                }
            }
            if (switch3.classList[1] == 'desactivado' && (switch1.classList[1] == 'activado' || switch2.classList[1] == 'activado')) {
                for (const value of items.values()) {
                    if (value.classList[1] == 'gobernanza') {
                        value.classList.add("Quitar")
                        console.log("hola")
                    }
                }
                switch3.classList.remove("activado")
                switch3.classList.add("desactivado")
            }
        }
    }
}
</script>