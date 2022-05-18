<template>
    <section>
        <div class="core text-center">
            <h4>our core values</h4>
            <hr>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea distinctio ipsa veniam ratione sit tempore asperiores assumenda aliquam perferendis beatae.</p>
            <div class="container-card">
                <div class="row">
                    <div class="card col-3">
                        <i class="fa-solid fa-house-chimney"></i>
                        <div class="text">
                            <h5>great services</h5>
                            <hr>
                            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis quasi doloribus architecto iure alias laboriosam dolorum! Modi voluptatibus quibusdam odio!</span>
                        </div>
                    </div>
                    <div class="card col-3">
                        <i class="fa-solid fa-gear"></i>
                        <div class="text">
                            <h5>highest standards</h5>
                            <hr>
                            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis quasi doloribus architecto iure alias laboriosam dolorum! Modi voluptatibus quibusdam odio!</span>
                        </div>
                    </div>
                    <div class="card col-3">
                        <i class="fa-solid fa-users"></i>
                        <div class="text">
                            <h5>professional team</h5>
                            <hr>
                            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis quasi doloribus architecto iure alias laboriosam dolorum! Modi voluptatibus quibusdam odio!</span>
                        </div>
                    </div>
                    <div class="card col-3">
                        <i class="fa-regular fa-lightbulb"></i>
                        <div class="text">
                            <h5>creative solutions</h5>
                            <hr>
                            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis quasi doloribus architecto iure alias laboriosam dolorum! Modi voluptatibus quibusdam odio!</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppCore'
}
</script>

<style lang="scss">
@import '../style/vars';
section{
    background-color: $bg-main;
    .core{
        width: 80%;
        margin: 0 auto;
        padding: 50px 0;
        h4{
            text-transform: uppercase;
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
        .container-card{
            width: 100%;
            .card{
                background-color: $bg-main;
                color: $text-color;
                padding: 0;
                border: none;
                text-align: center;
                i{
                    padding: 30px 0;
                    color: $text-color-title;
                    font-size: 40px;
                }
                .fa-house-chimney{
                    background-color: $bg-home;
                    line-height: 20px;
                    vertical-align: middle;
                    width: 80px;
                    border-radius: 50%;
                    margin: 10px auto;
                }
                .fa-gear{
                    background-color: $bg-settings;
                    line-height: 20px;
                    vertical-align: middle;
                    width: 80px;
                    border-radius: 50%;
                    margin: 10px auto;
                }
                .fa-users{
                    background-color: $bg-users;
                    line-height: 20px;
                    vertical-align: middle;
                    width: 80px;
                    border-radius: 50%;
                    margin: 10px auto;
                }
                .fa-lightbulb{
                    background-color: $bg-bulb;
                    line-height: 20px;
                    vertical-align: middle;
                    width: 80px;
                    border-radius: 50%;
                    margin: 10px auto;
                }
                .text{
                    padding: 10px;
                    h5{
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
}
</style>