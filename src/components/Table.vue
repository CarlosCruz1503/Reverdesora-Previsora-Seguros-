<template>
    <div class="container">
        <div class="t-claves">
            <p class="t-gray">Nosotros</p>
            <h1 class="t-h1" id="th">¿Por qué asegurarte con nosotros?</h1>
        </div>
        <div class="row">
            <div class="col-12 col-md-2"></div>
            <div class="col-0 col-md-8">
                <div class="t-table">
                    <table class="table">
                        <thead class="t-head">
                            <tr>
                                <th scope="col">
                                    <p> Beneficios</p>
                                </th>
                                <th scope="col"></th>
                                <th scope="col"></th>
                                <th scope="col"></th>
                                <th scope="col" class="th-img"><img src="../../public/img/logo-previsora.png" alt="">
                                </th>
                                <th scope="col" class="th-venta">
                                    <p>Otros Seguros</p>
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <Tr img="https://cdn-icons-png.flaticon.com/512/2997/2997187.png"
                                BText="Bonos verdes"
                                BDescripcion="Toda tu inversión, estará destianda a tus propios proyects y a cuidar el planeta" />
                            <Tr img="https://img.freepik.com/vector-gratis/dibujado-mano-dia-mundial-medio-ambiente-salva-planeta-ilustracion_52683-61570.jpg?w=2000g"
                                BText="Flexibilidad"
                                BDescripcion="Paquete de seguros que se acomoda a tus necesidades" />
                            <Tr img="https://img.freepik.com/vector-gratis/ilustracion-plana-dia-mundial-medio-ambiente_23-2149412970.jpg?w=2000"
                                BText="Empresas que se pueden asegurar"
                                BDescripcion="Todo tipo de empresas que cumplan la taxonomia verde" />
                            <Tr img="https://static.vecteezy.com/system/resources/previews/005/907/671/non_2x/illustration-graphic-cartoon-character-of-care-for-the-earth-and-the-environment-vector.jpg"
                                BText="Aliados"
                                BDescripcion="Contar con cadena de aliados, para formulación, ejecución, financiación y asesorias durante todo el proceso​" />
                        </tbody>
                    </table>
                </div>
            </div>
            <div class="col-12  text-final">
                <p>Entre muchos otros</p>
                <p class="text-desc">(Nuestro seguro es muy personalizable y sus coberturas y asistencias tambien)</p>
            </div>
        </div>
    </div>
</template>

<script>
import Tr from './TrTable.vue'
export default {
    name: 'Table',
    components: {
        Tr,
    }
}
</script>