<template>
    <div class="card card-card" >
        <div class="row g-0 r-card">
            <div class="col-md-4 icon">
                <img :src=icon class="i-icon">
            </div>
            <div class="col card-size">
                <div class="card-body">
                    <h5 class="card-title">{{ title }}</h5>
                    <p class="card-text">{{ text }}</p>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'CardClave',
    props: {
        title: String,
        text: String,
        icon: String,
    }
}
</script>