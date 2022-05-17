<template>
    <div class="partners text-center">
        <h4>trusted partners</h4>
        <hr>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea distinctio ipsa veniam ratione sit tempore asperiores assumenda aliquam perferendis beatae.</p>
        <div class="images-container">
            <div class="row row-cols-5" v-for="(item, index) in partners" :key="index">
                <img :src="'./images/partners/' + item.image" :alt="item.title">
            </div>
        </div>  
    </div>
</template>

<script>
import dati from "../partners.json"
export default {
    name: 'AppPartners',
    data(){
        return{
            partners: dati
        }
    }
}
</script>

<style lang="scss">
@import '../style/vars';
.partners{
    width: 80%;
    margin: 50px auto;
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
    .images-container{
        width: 90%;
        margin: 0 auto;
        display: flex;
        align-items: center;
        div{
            width: 100%;
            img{
                width: 100%;
            }
        }
    }
}
</style>