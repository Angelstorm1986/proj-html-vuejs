<template>
    <section>
        <div class="top-specialist text-center">
            <h3>do you have a construction project we can help with?</h3>
            <button>get a free quote</button>
        </div>
        <div class="specialist text-center">
            <h4>specialist in modern construction</h4>
            <hr>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea distinctio ipsa veniam ratione sit tempore asperiores assumenda aliquam perferendis beatae.</p>
        </div>
        <div class="container-card">
                <div class="row">
                    <div class="card col-3">
                        <i class="fa-solid fa-building"></i>
                        <div class="text">
                            <h4>buildings</h4>
                            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis quasi doloribus architecto iure alias laboriosam dolorum! Modi voluptatibus quibusdam odio!</span>
                        </div>
                    </div>
                    <div class="card col-3">
                        <i class="fa-solid fa-arrows-rotate"></i>
                        <div class="text">
                            <h4>renovate</h4>
                            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis quasi doloribus architecto iure alias laboriosam dolorum! Modi voluptatibus quibusdam odio!</span>
                        </div>
                    </div>
                    <div class="card col-3">
                        <i class="fa-solid fa-house-chimney"></i>
                        <div class="text">
                            <h4>construct</h4>
                            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis quasi doloribus architecto iure alias laboriosam dolorum! Modi voluptatibus quibusdam odio!</span>
                        </div>
                    </div>
                    <div class="card col-3">
                        <i class="fa-solid fa-truck"></i>
                        <div class="text">
                            <h4>exclusive</h4>
                            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis quasi doloribus architecto iure alias laboriosam dolorum! Modi voluptatibus quibusdam odio!</span>
                        </div>
                    </div>
                </div>
            </div>
    </section>
</template>

<script>
export default {
    name: 'AppSpecialist'
}
</script>

<style lang="scss">
@import '../style/vars';
section{
    background-color: $bg-standard;
    .top-specialist{
        height: 100px;
        background-color: $bg-top-specialist;
        text-transform: capitalize;
        position: relative;
        button{
            @include button-layout;
            background-color: $bg-button-secondary;
            color: $text-color-title;
            position: absolute;
            bottom: -50%;
            transform: translate(-75%, -100%);
        }
    }
    .specialist{
        width: 80%;
        margin: 0 auto;
        padding: 50px 0;
        h4{
            text-transform: capitalize;
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
            color: $text-color;
        }
    }
    .container-card{
        width: 100%;
        padding: 50px 0;
        .card{
            color: $text-color;
            padding: 0;
            border: none;
            text-align: center;
            i{
                padding: 30px 0;
                font-size: 40px;
            }
            .fa-building{
                border: 1px solid $text-color;
                line-height: 20px;
                vertical-align: middle;
                width: 80px;
                border-radius: 50%;
                margin: 10px auto;
            }
            .fa-arrows-rotate{
                border: 1px solid $text-color;
                line-height: 20px;
                vertical-align: middle;
                width: 80px;
                border-radius: 50%;
                margin: 10px auto;
            }
            .fa-house-chimney{
                border: 1px solid $text-color;
                line-height: 20px;
                vertical-align: middle;
                width: 80px;
                border-radius: 50%;
                margin: 10px auto;
            }
            .fa-truck{
                border: 1px solid $text-color;
                line-height: 20px;
                vertical-align: middle;
                width: 80px;
                border-radius: 50%;
                margin: 10px auto;
            }
            .text{
                padding: 10px;
                h4{
                    font-size: 1.40rem;
                    text-transform: capitalize;
                }
                p{
                    margin: 0 auto;
                }
                hr{
                    width: 20%;
                    margin: 20px auto;
                    color: $text-color;
                    height: 1px;
                }
            }
        }
    }
}
</style>