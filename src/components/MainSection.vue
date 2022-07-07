<template>
    <section>
        <div class="container">

            <div class="series">
                CURRENT SERIES
            </div>

            <div class="products-list">
                <MainCard v-for="element, index in dcProduct" :key="index" :DcproductDetails="element" />
            </div>

            <div class="more">
               <a href="#">LOAD MORE</a> 
            </div>
        </div>
    </section>
</template>

<script>

import comicsJson from '../assets/dc-comics.json';
import MainCard from './MainCard.vue';

export default {
    name: "MainSection",
    components: {
        MainCard
    },
    data() {
        return {
            dcProduct: comicsJson
        };
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

section {
    padding: 30px 0;
    background-color: $brand_secondary_color;
    position: relative;

        .series{
            position: absolute;
            bottom: calc((100% - 10px) - 12px) ;
            color: white;
            font-size: 15px;
            font-weight: bolder;
            background-color: $brand_primary_color;
            padding: 18px

        };

        .products-list {
            display: flex;
            flex-wrap: wrap;
        };

        .more{
            width: 20%;
            margin: 0 auto;
            color: white;
            font-size: 15px;
            padding: 10px;
            text-align: center;
            font-weight: bolder;
            background-color: $brand_primary_color;
        }
    }
    
  

</style>