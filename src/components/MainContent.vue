<template>
    <section>
        <div class="container">
            <span>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="Dc logo">

                <a href="#">DIGITAL COMICS</a>
            </span>

            <span>
                <img src="../assets/img/buy-comics-merchandise.png" alt="Dc logo">

                <a href="#">DIGITAL COMICS</a>
            </span>

             <span>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="Dc logo">

                <a href="#">DIGITAL COMICS</a>
            </span>

             <span>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="Dc logo">

                <a href="#">DIGITAL COMICS</a>
            </span>

             <span>
                <img src="../assets/img/buy-dc-power-visa.svg" alt="Dc logo">

                <a href="#">DIGITAL COMICS</a>
            </span>
        </div>
    </section> 
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
section{
    background-color: $brand_primary_color;
}

.container{
    padding: 35px;
    display: flex;

    span{
        display: flex;
        align-items: center;
        padding: 0 20px;

        img{
            width: 40px;
            height: 55px;
        }

        a{
            font-size: 14px;
            text-align: center;
            padding-left: 10px;
            color: white;
            text-decoration: none;
        }
    }
}

</style>