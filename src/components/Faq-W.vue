<template>
    <div class="accordion-item">
        <h2 class="accordion-header" :id=name>
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" :data-bs-target=ANameNumber
                aria-expanded="true" :aria-controls=nameNumber>
                {{FaqT}}
            </button>
        </h2>
        <div :id=nameNumber class="accordion-collapse collapse" :aria-labelledby=name
            data-bs-parent="#accordionExample">
            <div class="accordion-body">
                {{Answer}}
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name: 'FaqQ',
    props: {
        name: String,
        nameNumber: String,
        ANameNumber: String,
        number: String,
        FaqT: String,
        Answer: String
    }
}
</script>