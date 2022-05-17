<template>
    <div class="container-jumbo">
        <div class="img-jumbo">
            <img src="../assets/images/home-slider-62528242.webp" alt="Construction">
            <div class="demos">
                <i class="fa-solid fa-box-archive"></i>
                <p>demos</p>
            </div>
            <div class="sale">
                <div class="dollar">
                    <i class="fa-solid fa-dollar-sign"></i>
                    <span>39</span>
                    <p>on sale</p>
                </div>
            </div>
            <div class="title">
                <h1>building inspiring spaces</h1>
                <p>we build inspiring residential & commerciale spaces</p>
                <div>
                    <button class="explore-title">explore recent work</button>
                    <button class="quote-title">get a quote today</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'AppJumbotron'
}
</script>

<style lang="scss">
@import '../style/vars';
.container-jumbo{
    width: 100%;
    height: 100vh;
    .img-jumbo{
    position: relative;
    @include cover;
        img{
            @include cover;
        }
        .demos{
            @include label-jumbo;
            top: 15px;
            right: 15px;
            .fa-box-archive{
                font-size: 25px;
            }
        }
        .sale{
            @include label-jumbo;
            top: 85px;
            right: 15px;
            .dollar{
                color: $label-text;
                text-align: center;
                .fa-dollar-sign{
                    float: left;
                    font-weight: bold;
                }
                span{
                    font-size: 25px;
                    font-weight: bold;
                }
                p{
                color: $text-color;
                font-size: 10px;
                }
            }
        }
        .title{
            position: absolute;
            top: 50%; 
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            h1{
                text-transform: uppercase;
                color: $text-color-title;
            }
            p{
                text-transform: capitalize;
                color: $text-color-alternative;
            }
            .explore-title{
                @include button-layout;
                background-color: $bg-button-secondary;
                color: $text-color-title;
            }
            .quote-title{
                @include button-layout;
                background-color: $bg-button-standard;
                color: $text-color;
            }
        }
    }
}
</style>