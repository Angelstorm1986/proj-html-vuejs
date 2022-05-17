<template>
    <footer>
        <div class="top-footer">
            <img src="../assets/images/about-call-to-action-57862405.jpg" alt="About call to action">
            <div class="top-footer-container">
                <div class="row d-flex align-items-center">
                    <div class="col-8">
                        <h4>building inspiring spaces</h4>
                        <hr>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus esse veniam nihil iure! Omnis quo, quae cupiditate quas amet doloremque!</p>
                    </div>
                    <div class="row-right col-4 text-center">
                        <button>get a free quote</button>
                        <p>Only takes a few seconds!</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="mid-footer">

        </div>
        <div class="bottom-footer">
            <div class="copyright">
                <p>copyright 2012 - 2015 avada theme by <span>theme fusion</span> | all rights reserved | powered by <span>wordpress</span></p>
            </div>
            <div class="social">
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-youtube"></i>
                <i class="fa-brands fa-instagram"></i>
            </div>
            <button class="start">
                <i href="#" class="fa-solid fa-angle-up"></i>
            </button>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'AppFooter'
}
</script>

<style lang="scss">
@import '../style/vars';
.top-footer{
    width: 100%;
    height: 300px;
    position: relative;
    img{
        width: 100%;
        height: 100%;
    }
    .top-footer-container{
        width: 70%;
        margin: 0 auto;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        h4{
            text-transform: capitalize;
            color: $text-color-title;
        }
        hr{
            width: 20%;
            height: 2px;
            opacity: 1;
            margin: 30px 0;
            color: $text-color-alternative;
        }
        p{
            color: $text-color-title;
        }
        button{
            @include button-layout;
            background-color: $bg-button-standard;
            color: $text-color;
        }
        .row-right p{
            color: $text-color-title;
            font-size: 10px;
            margin-top: 10px;
        }
    }
}

.bottom-footer{
    width: 100%;
    height: 50px;
    background-color: $bg-footer-bottom;
    color: $text-color;
    text-transform: uppercase;
    font-size: 10px;
    @include my-flex;
    padding: 0 20px;
    position: relative;
    p{
        margin: 0;
    }
    .copyright span{
        color: $text-color-light;
    }
    .social{
        margin-right: 50px;
        font-size: 15px;
        i{
            padding-left: 10px;
        }
    }
    .start{
        position: absolute;
        bottom: 0;
        right: 5px;
        width: 40px;
        height: 25px;
        border-radius: 5px;
        background-color: $bg-button-footer;
        color: $text-color-title;
    }
}
</style>