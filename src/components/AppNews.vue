<template>
    <section>
        <div class="news text-center">
            <h4>latest news</h4>
            <hr>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea distinctio ipsa veniam ratione sit tempore asperiores assumenda aliquam perferendis beatae.</p>
            <div class="container-card">
                <div class="row">
                    <div class="card" v-for="(item, index) in news" :key="index">
                        <img :src="'./images/news/' + item.image" :alt="item.title">
                        <div class="card-text">
                            <h5>{{ item.title }}</h5>
                            <p>{{ item.date }}</p>
                            <hr>
                            <span>{{ item.description }}</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import dati from "../news.json"
export default {
    name: 'AppNews',
    data(){
        return{
            news: dati
        }
    }
}
</script>

<style lang="scss">
@import '../style/vars';
section{
    background-color: $bg-main;
    .news{
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