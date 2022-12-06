<template>
  <div class="container">
    <nav class="nav">
      <div class="logo">
        <img src="../public/img/logo-reverdesora.png" alt="logo">
      </div>
      <div class="solicitud">
        <button class="p-solicitud" data-bs-toggle="modal" data-bs-target="#exampleModal">¿Por qué asegurar?</button>
        <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
          <div class="modal-dialog">
            <div class="modal-content">
              <div class="row">
                <div class="col-12 col-md-6 col-xl-4">
                  <div class="card  mb-3" style="width: auto;">
                    <div class="card-header">NECESIDAD DE ASEGURAR LA INVERSIÓN EN IMPLEMENTAR PROYECTOS ASG
                    </div>
                    <div class="card-body">
                      <p class="card-text">* Para las organizaciones es fundamental invertir en forma confiable y
                        protegerse de los distintos riesgos asociados a la implementación de los proyectos ASG o
                        cualquier otro impacto negativo que pueda surgir antes, durante o después del mismo.
                      </p>
                    </div>
                  </div>
                </div>
                <div class="col-12 col-md-6 col-xl-4">
                  <div class="card  mb-3" style="width: auto;">
                    <div class="card-header">NECESIDAD DE INCORPORACIÓN DE CRITERIOS ASG COMO FACTOR ESTRATÉGICO
                    </div>
                    <div class="card-body">
                      <p class="card-text">* Lo criterios ASG buscan crear bienestar y desarrollo sostenible.
                      </p>
                      <p class="card-text">* Igualmente para los inversionistas, la selección de sus portafolios ya no
                        está basada únicamente en la rentabilidad sino que también se han incorporado factores como la
                        generación de valor, enmarcada en la sostenibilidad de los negocios y grupos de interés.

                      </p>
                    </div>
                  </div>
                </div>
                <div class="col-12 col-md-6 col-xl-4">
                  <div class="card y mb-3" style="width:auto;">
                    <div class="card-header">NECESIDAD DE INCORPORAR CRITERIOS ASG DE MANERA INTEGRAL
                    </div>
                    <div class="card-body">

                      <p class="card-text">* Abordar las iniciativas en forma individual, retrasa el cumplimiento
                        estratégico y expone de mayor manera a las organizaciones a la pérdida de valor por lo que se
                        requiere habilitar una estrategia que de sentido de urgencia a la ejecución de un portafolio
                        balanceado en términos ambientales, sociales y de Gobernanza.
                      </p>
                    </div>

                  </div>
                </div>
                <div class="d-button">
                  <button type="button" class="btn btn-success close" data-bs-dismiss="modal">Close</button>
                </div>

              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="buttons">
        <a href="#radar" class="">Cómo Funciona?</a>
        <a href="#claves" class="">Beneficios?</a>
        <a href="#services" class="">Servicios</a>
      </div>

    </nav>
  </div>
  <router-view />
</template>

<style lang="scss">

</style>
