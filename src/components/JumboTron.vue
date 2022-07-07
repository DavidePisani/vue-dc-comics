<template>
    <section class="jumbotron">

         <img src="../assets/img/jumbotron.jpg" alt="Dc logo">
    </section>
    
</template>

<script>
export default {
    name: 'JumboTron',
}
</script>

<style lang="scss" scoped>

.jumbotron{
  position: relative;
  height: 500px;
  width: 100%;

    img{
        height: 100%;
        object-fit: cover;
        object-position: top;
        width: 100%;
    }
}

</style>