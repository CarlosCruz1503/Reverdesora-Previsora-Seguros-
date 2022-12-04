<template>
    <tr class="tr-control">
        <th scope="row" class="benefits">
            <div class="img-benefits">
                <img :src=img alt="">
            </div>
            <div class="t-benefits">
                <p class="b-title">{{ BText }}</p>
                <p class="b-description">{{ BDescripcion }}</p>
            </div>
        </th>
        <td></td>
        <td></td>
        <td></td>
        <td class="td-c-img">
            <div class="div-td-img">
                <img class="correct-img" src="../../public/img/correct.png" alt="">
            </div>
        </td>
        <td class="td-T">
            <div class="div-p">
                <p class="x">X</p>
            </div>
        </td>
    </tr>
</template>
<script>
export default {
    name: 'Tr',
    props: {
        img: String,
        BText: String,
        BDescripcion: String
    }
}
</script>