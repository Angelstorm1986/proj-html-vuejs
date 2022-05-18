<template>
<div class="image-container">
    <div class="half-circle">
        <svg class="half-circle-top" xmlns="http://www.w3.org/2000/svg" version="1.1" width="100%" height="100" viewBox="0 0 100 100" preserveAspectRatio="none" style="padding:0;" fill="rgba(240,237,230,1)"><path d="M0 0 C55 180 100 0 100 0 Z"></path></svg>
        <svg class="half-circle-bottom" xmlns="http://www.w3.org/2000/svg" version="1.1" width="100%" height="100" viewBox="0 0 100 100" preserveAspectRatio="none" style="padding:0;" fill="rgba(240,237,230,1)"><path d="M0 100 C40 0 60 0 100 100 Z"></path></svg>
    </div>
    <img :src="require('../assets/images/home-parallax-144609983.jpg')" alt="Home">
    <div class="home text-center">
        <h4>our home owners say</h4>
        <hr>
        <img :src="require('../assets/images/home-testimonial-84268399.jpg')" alt="">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea distinctio ipsa veniam ratione sit tempore asperiores assumenda aliquam perferendis beatae.</p>
        <span>harry smith - new home owner</span>
    </div>
</div>
</template>

<script>
export default {
    name: 'AppHome'
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
    .home{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 80%;
        margin: 0 auto;
        color: $text-color-title;
        h4{
            text-transform: capitalize;
        }
        img{
            width: 100px;
            height: 100px;
            border-radius: 50%;
        }
        hr{
            width: 15%;
            margin: 30px auto;
            height: 2px;
            opacity: 1;
            color: $text-color-alternative;
        }
        p{
            width: 80%;
            margin: 30px auto;
        }
        span{
           text-transform: uppercase; 
        }
    }
}
</style>