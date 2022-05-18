<template>
    <div class="image-container">
        <div class="half-circle">
            <svg class="half-circle-top" xmlns="http://www.w3.org/2000/svg" version="1.1" width="100%" height="100" viewBox="0 0 100 100" preserveAspectRatio="none" style="padding:0;" fill="rgba(255,255,255,1)"><path d="M0 0 C55 180 100 0 100 0 Z"></path></svg>
            <svg class="half-circle-bottom" xmlns="http://www.w3.org/2000/svg" version="1.1" width="100%" height="100" viewBox="0 0 100 100" preserveAspectRatio="none" style="padding:0;" fill="rgba(255,255,255,1)"><path d="M0 100 C40 0 60 0 100 100 Z"></path></svg>
        </div>
        <img :src="require('../assets/images/home-244125289.jpg')" alt="Home">
        <div class="results text-center d-flex justify-content-center">
            <div>
                <i class="fa-solid fa-suitcase"></i><br>
                <span>3534</span>
                <p>planning applications</p>
            </div>
            <div>
                <i class="fa-solid fa-building"></i><br>
                <span>896</span>
                <p>completed projects</p>
            </div>
            <div>
                <i class="fa-solid fa-users"></i><br>
                <span>172</span>
                <p>trained professionals</p>
            </div>
            <div>
                <i class="fa-solid fa-globe"></i><br>
                <span>19</span>
                <p>international offices</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'AppResults'
}
</script>

<style lang="scss">
@import '../style/vars';
.image-container{
    width: 100%;
    height: 600px;
    position: relative;
    background-color: $bg-main;
    img{
        width: 100%;
        height: 100%;
    }
    .half-circle-top{
        position: absolute;
        top: 0;
    }
    .half-circle-bottom{
        position: absolute;
        bottom: 0;
    }
    .results{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 80%;
        margin: 0 auto;
        color: $text-color-alternative;
        div{
            padding: 0 20px;
            i{
                font-size: 60px;
                padding-bottom: 10px;
            }
            span{
                font-size: 50px;
            }
            p{
                text-transform: uppercase;
                color: $text-color-title;
            }
        }
    }
}
</style>