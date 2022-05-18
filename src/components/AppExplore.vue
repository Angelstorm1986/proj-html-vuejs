<template>
    <section>
        <div class="explore text-center">
            <h4>explore recent work</h4>
            <hr>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea distinctio ipsa veniam ratione sit tempore asperiores assumenda aliquam perferendis beatae.</p>
            <div class="container-card">
                <div class="row">
                    <div class="card">
                        <img :src="'./images/explore/project2-featured-15013609-800x800.jpg'" alt="Electric Plant">
                    </div>
                    <div class="card">
                        <img :src="'./images/explore/project1-featured-294276386-800x800.jpg'" alt="Beautiful Villa">
                    </div>
                    <div class="card">
                        <img :src="'./images/explore/project3-featured-189023420-800x800.jpg'" alt="Residential">
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppExplore'
}
</script>

<style lang="scss" scoped>
@import '../style/vars';
section{
    background-color: $bg-standard;
    .explore{
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
        }
        .container-card{
            width: 100%;
            .card{
                width: calc((100% / 3) - 40px);
                margin: 0 10px;
                color: $text-color;
                padding: 0;
                border: none;
                text-align: left;
                .card-text{
                    padding: 10px;
                    h5{
                        font-size: 1.40rem;
                    }
                    p{
                        margin: 0 auto;
                    }
                    hr{
                        width: 95%;
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