<template>
    <header>
        <div class="logo">
            <img src="../assets/images/construction_mobile_logo.png" alt="Avada Constructions Logo">
        </div>
        <nav>
            <div>
                <ul>
                    <header-data v-for="(item, index) in navbar" :key="index" :text="item.text" :active="item.active"/>
                </ul>
                <button class="standard-button">get quote</button>
            </div>
        </nav>           
    </header>
</template>

<script>
import dati from "../navBar.json"
import HeaderData from './HeaderData.vue'
export default {
    name: 'AppHeader',
    components:{
        HeaderData
    },
    data(){
        return{
            navbar: dati
        }
    }
}
</script>

<style lang="scss">
@import '../style/vars';
header{
    height: 100px;
    @include my-flex;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    background-color: $bg-standard;
    z-index: 1;
    .logo{
        margin-left: 50px;
    }
    nav div{
        @include my-flex;
        ul{
            @include my-flex;
            padding-top: 15px;
            li{
                list-style-type: none;
                padding: 0 10px;
                line-height: 120px;
                z-index: 1;
                a{
                    text-decoration: none;
                    text-transform: uppercase;
                    color: $bg-footer;
                    font-weight: bold;
                    .choice{
                        position: relative;
                    }
                    .active{
                        color: $bg-button-standard;
                        &::after{
                            position: absolute;
                            bottom: 8px;
                            content: '';
                            width: 100%;
                            height: 3px;
                            background-color: $bg-button-standard;
                        }
                    }
                }
            }
        }
        .standard-button{
            @include button-layout;
            background-color: $bg-button-standard;
            color: $text-color;
        }
    }
}
</style>