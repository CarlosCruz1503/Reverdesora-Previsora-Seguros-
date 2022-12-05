<template>
    <button :id=name class="radar-item Quitar" :class=grup type="button" data-bs-toggle="modal" :data-bs-target=targetA  >
        {{Title}}
        <i class="bi bi-award-fill"></i>
    </button>
    <div class="modal fade" :id=target tabindex="-1" :aria-labelledby=nameLabel aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
                <div class="modal-header">
                    <h1 class="modal-title fs-5" :id=nameLabel >  {{Title}} </h1>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    {{Description}}
                    <br>
                    Costos : {{Costo}}M 
                </div>
                <div class="modal-footer">
                    
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
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
        Description:String,
        grup:String,
        Costo:String
    }
}
</script>