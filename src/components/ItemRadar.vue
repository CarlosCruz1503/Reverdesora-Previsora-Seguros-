<template>
    <button :id=name class="radar-item Quitar" :class=grup type="button" data-bs-toggle="modal" :data-bs-target=targetA  >
        {{Title}}
        <i class="bi bi-award-fill"></i>
    </button>
    <div class="modal fade" :id=target tabindex="-1" :aria-labelledby=nameLabel aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header">
                    <img class="modal-icon" :src=img>
                    <h1 class="modal-title fs-5" :id=nameLabel >  {{Title}} </h1>
                    
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <h4 class="modal-body-title">¿Qué cubrimos?
                    </h4>
                    <p>{{cubrimos1}}</p>
                    <p>{{cubrimos2}}</p>
                    <p>{{cubrimos3}}</p>
                    <p>{{cubrimos4}}</p>
                    <p>{{cubrimos5}}</p>
                </div>
                <div class="modal-body">
                    <h4 class="modal-body-title">¿Qué no cubrimos?

                    </h4>
                    <p>{{noCubrimos1}}</p>  
                    <p>{{noCubrimos2}}</p>  
                    <p>{{noCubrimos3}}</p>  
                    <p>{{noCubrimos4}}</p>  
                    <p>{{noCubrimos5}}</p>  
                </div>
                <div class="modal-body">
                    <h4 class="modal-body-title">Asistencias
                    </h4>
                    <p>{{asistencias1}}</p>
                    <p>{{asistencias2}}</p>
                    <p>{{asistencias3}}</p>
                    <p>{{asistencias4}}</p>
                    <p>{{asistencias5}}</p>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary close-gray"  data-bs-dismiss="modal">Close</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ItemRadar',
    props: {
        name:String,
        targetA:String,
        target:String,
        nameLabel:String,
        Title:String,
        cubrimos1:String,
        cubrimos2:String,
        cubrimos3:String,
        cubrimos4:String,
        cubrimos5:String,
        noCubrimos1:String,
        noCubrimos2:String,
        noCubrimos3:String,
        noCubrimos4:String,
        noCubrimos5:String,
        asistencias1:String,
        asistencias2:String,
        asistencias3:String,
        asistencias4:String,
        asistencias5:String,
        grup:String,
        Costo:String,
        img:String,
    }
}
</script>