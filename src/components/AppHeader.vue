<template>
    <header>
        <div class="logo">
            <img src="../assets/images/construction_mobile_logo.png" alt="Avada Constructions Logo">
        </div>
        <nav>
            <div>
                <ul>
                    <li v-for="(item, index) in navbar" :key="index">
                        <a href="#">
                            <div class="choice" :class="{ active : item.active }">{{item.text}}</div>
                        </a>
                    </li>
                </ul>
                <button class="standard-button">get quote</button>
            </div>
        </nav>           
    </header>
</template>

<script>
import dati from "../navBar.json"
export default {
    name: 'AppHeader',
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