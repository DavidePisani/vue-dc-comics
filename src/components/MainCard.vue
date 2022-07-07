<template>
    <div class="product-card">
        <img :src="DcproductDetails.thumb" :alt="DcproductDetails.series">
        <h3>{{ DcproductDetails.series }}</h3>
    </div>
</template>

<script>
export default {
    name: "MainCard",
    props: {
        DcproductDetails: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

.product-card {
    padding: 20px;
    width: calc((100% / 6) - 6px);
    margin: 0 auto;

    img{
        height: 190px;
        width: 100%;
    }

    h3 {
        margin-top: 3px;
        font-size: 13px;
        color: white
    }
}
</style>