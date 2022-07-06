<template>
  <header>
        <!-- Header logo -->
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="Dc logo">
            </div>

        <!-- Header nav -->
            <nav>
                <ul class="menu">
                    <li v-for="element, index in menuLinks" :key="index">
                        <a :href="element.url" :class="{'current': element.current }"> {{ element.text }} </a>
                    </li>
                </ul>
            </nav>
        </div> 
    </header>
 
</template>

<script>

export default {
  name: 'PageHeader',

    data(){
        return {
                menuLinks:[
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: false
                },

                {
                    text: 'COMICS',
                    url: '#',
                    current: true
                },

                {
                    text: 'MOVIES',
                    url: '#',
                    current: false
                },

                {
                    text: 'TV',
                    url: '#',
                    current: false
                },

                {
                    text: 'GAMES',
                    url: '#',
                    current: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false
                },
                {
                    text: 'VIDEO',
                    url: '#',
                    current: false
                },
                {
                    text: 'FUNS',
                    url: '#',
                    current: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: false
                },
            ],

        };
    }
  
}
</script>


<style lang="scss" scoped>
@import '../style/variables';

header {
        height: 100px;
        
        img{
            height: 100px;
        }
    
    .container{
        display: flex;
        justify-content: space-between;
        
    }

    nav{
        height: 100%;
    }

    .menu{
        display: flex;
        line-height: 100px;
    }
        li {
            padding: 0 10px;

            a {
                color: #606d77;
                text-decoration: none;
                font-size: 12px;
                font-weight: bolder;

                    &.current {
                        color:$brand_primary_color;
                        border-bottom: 3px solid $brand_primary_color ;
                        line-height: 100px;   
                    }  
            }

            
        }

}

</style>