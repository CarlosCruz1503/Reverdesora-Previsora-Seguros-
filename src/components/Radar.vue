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
                            asistencias1="* Asistencia de financiación de programas de gestión ambiental con nuestros aliados (Grupo Bicentenario). 
                            " asistencias2="* Asistencia con Ministerio de Ambiente y entidades involucradas para asesoramiento en implementación de programas de gestión ambiental.
                            " asistencias3="* Asistencia en mantenimiento de equipos de conservación ambiental e infraestructura. 
                            "
                            asistencias4="* Asistencia en talleres (pequeños accesorios y llantas estalladas – Vehículo de reemplazo)"
                            img="data:image/jpeg;base64,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" />

                        <ItemRadar name="adaptacionCClimatico" target="aCCTarget" targetA="#aCCTarget"
                            nameLabel="aCCLabel" Title="Adaptacion Cambio Climatico" grup="ambiental" Costo="100"
                            cubrimos1="* Amparo todo riesgo a equipos, maquinaria, insumos e infraestructura relacionados con proyectos de implementación de Adaptación al cambio climático en cualquier etapa de implementación (transporte, implementación y desarrollo)
                            " noCubrimos1="* Daños ambientales por incumplimiento doloso de normativa ambiental.
                            " asistencias1="* Asistencia de financiación de programas de gestión ambiental con nuestros aliados (Grupo Bicentenario). 
                            " asistencias2="* Asistencia con Ministerio de Ambiente y entidades involucradas para asesoramiento en implementación de programas de gestión ambiental.
                            " asistencias3="* Asistencia en mantenimiento de equipos de conservación ambiental e infraestructura. 
                            "
                            asistencias4="* Asistencia en talleres (pequeños accesorios y llantas estalladas – Vehículo de reemplazo)"
                            img="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAkGBwgHBgkIBwgKCgkLDRYPDQwMDRsUFRAWIB0iIiAdHx8kKDQsJCYxJx8fLT0tMTU3Ojo6Iys/RD84QzQ5Ojf/2wBDAQoKCg0MDRoPDxo3JR8lNzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzc3Nzf/wAARCABAAEADASIAAhEBAxEB/8QAGwAAAgIDAQAAAAAAAAAAAAAABgcEBQABAgP/xAA5EAABAwIFAwIFAQQLAQAAAAABAgMEBREABhIhMRNBUQdhFBUiI4EyQnGRoRYkM1ZykpWxwdHi8P/EABgBAAMBAQAAAAAAAAAAAAAAAAMEBQEC/8QAJhEAAQQCAgECBwAAAAAAAAAAAQACAxEEIRIxIkFRBRMUYZHh8P/aAAwDAQACEQMRAD8AZGdc3OZXdprTNKdqDk9xbaENOhCkqSARseb79xxhWyZubFRICa9nOFT32U/GMMvLS0717/Sh3ygC++/JBBsMZUJEdWe821pFOQw/Aiqdajz79fqoT/aoTwEHnk8gi17YJ8nZVpHyCLMnRI9Rmz2UyJMqSgOqcUsBRAJGw3tYeMSsvLe15a00BXpsnv8ACZiiBFlRKZnXM2Xpr5zC0KzGnvRxFlRlpbYaUu4KBtuAbW2ubXPOD3MSM3uTWhlp+itQ+n9xU5DqnNdzxpNrWt+cKup0qHTq1W8uMoi/LHaYakw3MUejDe1FFweUpN7+2JmTOrWPTiLTIz1UpSY6z/WI7xbU+rf6kr5KDfjbi3a+D4uS5/i/Zsb976/aDkcYhy9EZk+pcVWspyzPbHLaS8y4f3E3H8cXkGuul+mwarTpEOozGFOqbQC80yU8pU6Bpv8A/dxdQ5IVUqjTwYedqxGrbOpMmJIfEhLSkqIv019uO/fBfGzrU6OoQc+w2HKe99oVaGk9LfazyOU38jbf95wyJmF3G9oQcDpMhC0uISttQUhQulSTcEeRjrARVKinIUCkrpcBpeUW0lElbKlOOR9arpcG51IuTfk74NGnEPNIdaWlba0hSFpNwoHgg+MFXSUefqfKy9nNquqkSKjGq4UxKiCF1VNMISPpSRwDcbWFySTfFRRqhU6dT0NZXr1HdpnQMluPVioPQ2b7glB3SD544w1G67Jcz+9l8NM/BtUtMtTm+vqFwp082tbfi+Fw5lPJdTTINOhuQ41JnOtSXFHSXi3u4lRJN0ceLAbW3xPy8dt/Mur71dojZ+AohD9SqAjJnx41QVVK3UlMpnT0RQ7HbYWCAlIBIACTffn/AGupcebS00DKNPmyH32lpkvSirphMZCrFJAO4N7AewvjzpVcpcBMn+hmXKg6/OWFJuwWo6rXsrWf0p5NvftjqoU7MdTqVOn1VFIhCnu9VUqK471A2N1I32II8/8Ad+8PEkDw4tNXZOh/AeySysprgQSBo0vfMTkyl5ohVaDSJE8qhuxwI6L/AHCoFOs9k++NSKHmHMLam8y1VEOKU6fhKSSkLvzrUq9/FtxidTM4USpOKbbl/DrCdaUy09HqIPCk6uRi7S+ypnrpdbLJGrqBQ02834xc+lgkkMp2VHORNEwR1VKtyI58lqbuRqs4ZlJnR1rpqpFiSkD7rKvOxuNuL+bC89OHHqTKq+T5bi3DSHQuE4s3K4rm6BfvpN0n8DtgfqzKJ79FnQZ0NpyFUWnkPOPhKFJ4WnVvyDgyeochefoOY4amTGNOXEk/WbqGoLQUi1jvfuMLTsDH66VfDmMsQLuwq4kxfWUFezc6haUHytt65H+U3wvfktSnV/NdBVVfg6cKm48+wy0C66h76gNR/Ski388NPOUGE05AzPLffZNBLj5LDWtTjakaVot4O2/YA8cgY9QIyqVVYWdoDbjkB1hMeqISk3DR3Q9p5ukmx72sPOBsDC4cxYRMgPMZ4dqWwy3HYbYYQG2mkBCEJ4SkCwGB7ONWDdIEWnyYypM99ENJ1BWgOHSVWB3sMV9azBGzM0mgZakrkPTHA1JfbaUEsM8rVcixuBb84J4GVKBT3mnodJitvM20OaLqBHe57++C5vxBsPg3ZIUnHxCafJr7Lact0lNIhQZ8RiY1BZDaHJLYUQANz7XtfFLRqU7nR6murpiYuToyllpgu6TLI2QooHCAQbC+DBxCXW1tuC6FpKVDyDzhdz5uYMpR6XRJdXXFoSXFts1CHH6khQtdDaweDe+6Rv8AjEbDLS/yO/RVWUTtHKfTfKaam5O+UMnW2EfDndlJ7qCOAoiw8bcXuTX06VN9OJz8d6GXcoyZqRHeTI1Kp+sAEFJ36ev323O5NiL/AD8f30zN/pv/AIxOy5EzBn+HIp71SEnK6JyC5NlsaJMhCNKi0lIsLah+o7/wtimUZOrAtUprOU41RnZlqciZTJsxKW0rja0xULASUqKR+i/cjuBuTuU44dbbeaW08hLja0lKkKFwoHkEdxjFqWbmVKnRUmo5AkRqjRpH3RSnXvpF97sO8AHwduee0ZWcGohKK3RqzTHU7K60NS0H/CpNwR74IHchP0mQuVkisvUYrVrXBcT14iz3sg7ov5B44AxnzT1Fgo0ycuUiqLH7cGeWAfw4MAkxo5DZG1yWAoeTnSHJATSKZWKk4o2CY0FdvyVAAD3xznGnVeRkFVcmQH6ZVqdJTJYbadS6plAVYrVbY/QSSO1t8EYrHqHMQUx8q0umrPC5tS6yR+GxfEuFlutTodSYzdXRNbqEZTBixGA00wCNygm6ifc4yPGjYbHawMASpdzSwmOpxHqHVCQklJNJ2J7fs+ffDT9KKa5Tskw3JTTjc2cpcyV1TdS3Fm+o+LpCdu2FWxHzFOq6MmP1qoFPxaociJ8AlJRBTsHepa1ikbf8939CitQYbESOkpZYbS02Cb2SkWH8hhkrpf/Z" />

                        <ItemRadar name="PC" target="PCTarget" targetA="#PCTarget" nameLabel="PCLabel" Title="
                            Prevención accidentes" grup="social" Costo="20" convenio="
                            Convenio  con POSITIVA SEGUROS para la adquisición de seguros ramo vida – Riesgos Laborales
                            " cTitle="Convenio" img="https://cdn-icons-png.flaticon.com/512/503/503968.png"
                            imgConvenio="https://s3-ap-south-1.amazonaws.com/bot-bkt/prod/8931/Isologo_Positiva_avatar.png" />

                        <ItemRadar name="IS" target="ISTarget" targetA="#ISTarget" nameLabel="ISLabel" Title="
                        Infraestructura Social" grup="ambiental" Costo="200" cubrimos1="
                            * Amparo todo riesgo a infraestructura social (parques, bosques o cualquier otro espacio público que la empresa quiera asegurar y que beneficie a la comunidad, el ecosistema y las finanzas de la empresa)
" asistencias1="* Asistencia de financiación de programas de gestión de infraestructura social con nuestros aliados (Grupo Bicentenario). 
" asistencias2="* Asistencia con Ministerio de Ambiente y entidades involucradas para asesoramiento en implementación de programas de gestión social
" asistencias3="* Asistencia en mantenimiento de equipos de conservación ambiental e infraestructura social. 
" img="https://cdn-icons-png.flaticon.com/512/2942/2942548.png
" />

                        <ItemRadar name="GSC" target="GSCTarget" targetA="#GSCTarget" nameLabel="GSCLabel" Title="
                        Gestión de Stakeholders y comunidad" grup="ambiental" Costo="30" cubrimos1="
                            * Póliza de responsabilidad civil extracontractual por lesiones, muertes y/o daños materiales a bienes de terceros causados por el desarrollo normal de las actividades de la empresa:  
                            - Gastos de defensa
                            - Gastos Médicos de urgencia y/o funerarios
                            - Perdidas patrimoniales / Lucro cesante F
                     " noCubrimos1="* RC Contractual
                     " noCubrimos2="* Dolo o culpa grave
                     " img="https://cdn-icons-png.flaticon.com/512/2170/2170765.png
                     " />


                        <ItemRadar name="PEPL" target="PEPLTarget" targetA="#PEPLTarget" nameLabel="PEPLLabel" Title="
                        Promoción de empresas y pymes locales" grup="ambiental" Costo="15" cubrimos1="
                            * Póliza de seguro Daños combinados a centros comerciales, clústeres, parques industriales y zonas francas:
                            - Incendio
                            - Temblor – Terremoto
                            - Actos malintencionados – Terrorismo
                            - Sustracción con o sin violencia
                            - Corriente débil
                            - Rotura de maquinaria
                            - Lucro cesante
                    " img="https://cdn-icons-png.flaticon.com/512/6213/6213866.png
                    " />

                        <ItemRadar name="generacionEmpleo" target="gETarget" targetA="#gETarget" nameLabel="gELabel"
                            Title="Generación de empleo" grup="social" Costo="15" convenio="Convenio  con POSITIVA SEGUROS para la adquisición de seguros ramo vida – Riesgos Laborales
                            " cTitle="Convenio" img="https://img2.freepng.es/20181120/cba/kisspng-job-computer-icons-vector-graphics-illustration-em-5bf40ad62b7ba4.6073968715427202141781.jpg
                            "
                            imgConvenio="https://s3-ap-south-1.amazonaws.com/bot-bkt/prod/8931/Isologo_Positiva_avatar.png" />

                        <ItemRadar name="DT" target="DTTarget" targetA="#DTTarget" nameLabel="DTLabel"
                            Title="Derechos de los trabajadores" grup="social" Costo="15" convenio="Convenio  con POSITIVA SEGUROS para la adquisición de seguros ramo vida – Riesgos Laborales
                            " cTitle="Convenio" img="https://cdn-icons-png.flaticon.com/512/2694/2694564.png

                            "
                            imgConvenio="https://s3-ap-south-1.amazonaws.com/bot-bkt/prod/8931/Isologo_Positiva_avatar.png" />

                        <ItemRadar name="antiCorrupcion" target="aCTarget" targetA="#aCTarget" nameLabel="aCLabel"
                            Title="Anti-Corrupcion" grup="gobernanza" Costo="15" cubrimos1="* Póliza de seguro de cumplimiento sector público y/o sector privado en contratos suscritos: 
                            - Manejo de anticipos
                            - Cumplimiento de contratos
                            - Pago de salarios, prestaciones e indemnizaciones
                            - Estabilidad de obra y/o proyecto
                            " img="https://us.123rf.com/450wm/ahasoft2000/ahasoft20001704/ahasoft2000170402290/75440070-gratis-de-carga-icono-con-textura-granulada-dentro-del-c%C3%ADrculo-para-sellos-de-marca-de-agua-de-super.jpg?ver=6
                            " />

                        <ItemRadar name="CR" target="CRTarget" targetA="#CRTarget" nameLabel="CRLabel"
                            Title="Confianza y reputación" grup="gobernanza" Costo="20" cubrimos1="* Póliza de seguros para cubrir los gastos eventuales por daños a la imagen de la empresa asegurada: 
                            - Escandalo mediático
                            - Manejo inescrupuloso de redes sociales
                            - Ataques cibernéticos  
                            " noCubrimos1="* De acuerdo con apetito de riesgo de la aseguradora.
                            " img="https://cdn-icons-png.flaticon.com/512/1458/1458547.png
                            " />
                        <ItemRadar name="TJC" target="TJCTarget" targetA="#TJCTarget" nameLabel="TJCLabel"
                            Title="Trato justo a los clientes" grup="gobernanza" Costo="15" cubrimos1="* Póliza de responsabilidad civil extracontractual por lesiones, muertes y/o daños materiales a bienes de terceros causados por el desarrollo normal de las actividades de la empresa:   
                            - Gastos de defensa
                            - Gastos Médicos de urgencia y/o funerarios
                            - Perdidas patrimoniales / Lucro cesante 
                    " noCubrimos1="* RC Contractual
                    " noCubrimos2="* Dolo o culpa grave
                    " img="https://png.pngtree.com/png-vector/20220527/ourmid/pngtree-call-center-customer-icon-png-image_4746069.png
                    " />
                        <ItemRadar name="RC" target="RCTarget" targetA="#RCTarget" nameLabel="RCLabel"
                            Title="Rendicion de cuentas" grup="gobernanza" Costo="15" cubrimos1="* Póliza de seguros para cubrir los gastos eventuales por daños a la imagen de la empresa asegurada: 
                            - Escandalo mediático
                            - Manejo inescrupuloso de redes sociales
                            - Ataques cibernéticos  
                            " noCubrimos1="* De acuerdo con apetito de riesgo de la aseguradora.
                            " img="https://angelicalozano.co/wp-content/uploads/2018/09/iconos-05.png
                            " />

                        <ItemRadar name="OG" target="OGTarget" targetA="#OGTarget" nameLabel="OGLabel"
                            Title="Órganos de Gobierno" grup="gobernanza" Costo="150" cubrimos1="* Póliza de seguros para cubrir los gastos de eventuales daños antijurídicos que se produzcan por multas e incumplimiento de normatividad aplicable a la empresa. 
                            " noCubrimos1="* Incumplimiento doloso de normativa vigente .
                            " img="https://thetreeschool.org/wp-content/uploads/2015/05/icono-gobierno.png
                            " />






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

