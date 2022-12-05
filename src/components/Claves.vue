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
                " icon="https://static.wixstatic.com/media/805e91_65acf6947f8c4106b0d35b404a8df060~mv2.png/v1/crop/x_0,y_0,w_243,h_308/fill/w_85,h_108,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/growing%20plant.png" alt=""/>
                <CardClave title="2. Ajustable" text="Tanto las coberturas como las asistencias se acomodan a las iniciativas propuestas, el valor de la prima considera el valor del portafolio completo para aplicar tasas preferenciales.
                " icon="https://cdn-icons-png.flaticon.com/512/1063/1063333.png?w=900&t=st=1670213960~exp=1670214560~hmac=716e95a793770eda78c3024f65b3c58617c68a08455fd2e7b77a7eb67d70c3a0"/>
                <CardClave title="3. Asesoría
                " text="Acceso al directorio de aliados que pueden acompañarlo en la materialización de las iniciativas mapeadas.
                " icon="https://eter.edu.ar/images/iconos/donde-estamos.png"/>
                <CardClave title="4. Desempeño
                " text="Acceso a herramientas para la medición de los indicadores de desempeño en la gestión de los riesgos.
                " icon="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAD0AAAA9CAMAAAApvJHbAAAAaVBMVEVtEx////9kAABpABGZcXPNurtqBRdiAACHTlNrCRl/QEXd0tJgAABsDxxeAABmAABnAAv7+fnDqqyRXGHs4+S7n6GykpT28fLw6eqqhol+Nz56LjekfoDbzM23mZuhd3pzJC2WZWlxGya7TUmlAAACCklEQVRIid3XV5ODIBAA4AULamj202ja//+Rh6I3FjCRe7iZ26eE4cuKSwsg9NW0cD6uXYEQoJ5I5qCZRwMEqZMdPa4hw44YAN/g7jnrMAc/dNashUb+JndPnLUoASWuyWNRA0oTKj2HwKJXswWhoPPPx71M0ajd4691kQXnI5v1hePTQdof7TBh4uSsDoekgrlpLxrH+2Aumk3lKYiLjlutU/FOM0LFjovqM83UAsjoVpPyI83wRbVmfN3Ks4+eXGO0yU5H3L97a4xcplm85Bo/eXN7HVVMZ64btHp4/dg+BimPZovOnD54t8yuM98XW79RM9oPuPWALPgeGzUjM1YFambOg+FTt3o7Bq0zo0QfLxPndMTNujB7PeFo3qI1LzMDNmi8xmq81bwFVduZt9M42GCVfeK33bTdaTF8z9erQ2ffY3Pu5/Y0H7KXe2wYt8iv+zNNvF6m+4GhYqHpEsKMN5Pzu+J/04WD9p6zRm18WpPgR/f8ffd1yPHBp/M74Dg0xFDp2NDu0SRdaFTf8mgfVwahoTnyg2npHd4dKgk0PepwqNU9ktZ/pDsPaOGo03GnwKWbbvVi5wfcrkusTiWhfoHYh27X15jBpa4E4MxBcxADezBZWfvYtdQsZsI+cLv2PZBln3vA7UWz6y/CAOMQxNPa5ahiPVYnfUwie4/DuTb8QY3sL1zFN+j4I+l62lYdAAAAAElFTkSuQmCC"/>
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