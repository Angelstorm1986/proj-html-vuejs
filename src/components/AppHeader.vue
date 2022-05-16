<template>
    <header>
        <div class="logo">
            <img src="../assets/images/construction_mobile_logo.png" alt="Avada Constructions Logo">
        </div>
        <nav>
            <ul>
                <li v-for="(item, index) in navbar" :key="index">
                    <a href="#">
                        <div class="choice" :class="{ active : item.active }">{{item.text}}</div>
                    </a>
                </li>
            </ul>
            <div>
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
    nav{
        @include my-flex;
        ul{
            @include my-flex;
            line-height: 120px;
            }
            li{
                list-style-type: none;
                padding: 0 10px;
            a{
                text-decoration: none;
                text-transform: uppercase;
                color: $bg-footer;
                font-weight: bold;
                .choice{
                position: relative;
                display: flex;
                justify-content: center;
                // &:hover{
                //   color: $colortextactive;
                //   &::after{
                //     position: absolute;
                //     bottom: 0;
                //     content: '';
                //     width: 100%;
                //     height: 3px;
                //     background-color: $colortextactive;
                //   }
                // }
                }
            }
        }
        .standard-button{
            background-color: $bg-button-standard;
            color: $text-color;
            text-transform: uppercase;
            font-weight: bold;
            padding: 5px 20px;
            margin: 0 30px;
        }
    }
}
.active{
    color: $bg-button-standard;
    &::after{
        position: absolute;
        bottom: 0;
        content: '';
        width: 100%;
        height: 3px;
        background-color: $bg-button-standard;
    }
}
</style>