<template>
<footer>
    <div class="footer-top">
        <div class="container">
            <div class="list">
                <div>
                <ul>
                    <li><h3>DC COMICS</h3></li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                </ul>               
                <ul>
                    <li><h3>SHOP</h3></li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                </ul>
                </div>

                <ul>
                    <li><h3>DC</h3></li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                </ul>

                 <ul>
                    <li><h3>SITE</h3></li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                    <li>Lorem ipsum</li>
                </ul> 
            </div>

            <div class="bg-img">
               
            </div>
        
        </div>
    </div>

    <div class="footer-bottom">
        <div class="container">
           <div class="btn">
            <a href="#">SIGN-UP NOW!</a>
           </div>

           <div class="social">
            <h3>FOLLOW US</h3>
            <span><img src="../assets/img/footer-facebook.png" alt=""></span>
            <span><img src="../assets/img/footer-twitter.png" alt=""></span>
            <span><img src="../assets/img/footer-youtube.png" alt=""></span>
            <span><img src="../assets/img/footer-pinterest.png" alt=""></span>
            <span><img src="../assets/img/footer-periscope.png" alt=""></span>

           </div>
        </div>
        
    </div>
    
</footer>
    
</template>

<script>

export default {
     name: 'EndPage',
}

</script>

<style lang="scss" scoped>
@import '../style/variables';

.footer-top{
    background-image: url("../assets/img/footer-bg.jpg");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat; 
    color: white;

    .container{
        display: flex;
        justify-content: space-between;

        .list{
            width: 50%;
            display: flex;
            padding: 60px;
                li{
                    color: lightgrey;
                }

                ul{
                    padding-right: 40px;
                    padding-bottom: 15px
                }     
        }  

        .bg-img{
            background-image: url("../assets/img/dc-logo-bg.png");
            background-position: center;
            background-size: cover;
            width: 50%;
        }
    }   
}

.footer-bottom{
    background-color: $brand_secondary_color;

    .container{
        padding: 25px;
        display: flex;
        align-items: center;
        justify-content: space-between;

        .btn{
            border: 3px solid $brand_primary_color;

            a{
                padding: 15px;
                color: white;
                font-weight: bolder;
                display: inline-block;
            }
        }

        .social{
            display: flex;
            align-items: center;

            h3{
                color: $brand_primary_color;
                padding-right: 10px;
            }

            span{
                padding-right: 10px;
            }
        }
    }    
}

</style>