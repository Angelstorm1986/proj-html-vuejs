<template>
    <footer>
        <div class="top-footer">
            <img src="../assets/images/about-call-to-action-57862405.jpg" alt="About call to action">
            <div class="top-footer-container">
                <div class="row d-flex align-items-center">
                    <div class="col-8">
                        <h4>building inspiring spaces</h4>
                        <hr>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus esse veniam nihil iure! Omnis quo, quae cupiditate quas amet doloremque!</p>
                    </div>
                    <div class="row-right col-4 text-center">
                        <button>get a free quote</button>
                        <p>Only takes a few seconds!</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="mid-footer">
            <div class="mid-footer-container">
                <div class="row">
                    <div class="col-3">
                        <img src="../assets/images/footer-logo.png" alt="Avada Constructions Logo">
                        <p>We ara specialists in the construction of unique and exclusive properties. Our work inspires. We pride ourselves on delivering outstanding quality and design for leading clients across the world.</p>
                        <button>learn more</button>
                    </div>
                    <div class="col-3">
                        <div class="post">
                            <div class="post__header">
                                <h6>latest tweets</h6>
                                <div class="post-meta">                    
                                    <div class="post-meta__icon">
                                        <img class="profile-pic" src="../assets/images/3a74ce3d0532b7773b174c45ca3bd05a_normal.png" alt="Logo post">
                                        <div class="post-meta__data">
                                            <div class="post-meta__author">ThemeFusion</div>
                                            <div class="post-meta__profile">@Theme_Fusion</div>
                                        </div>
                                    </div>
                                    <div>
                                        <i class="fa-brands fa-twitter"></i>
                                    </div>
                                </div>
                            </div>
                            <div class="post__text">Placeat libero ipsa nobis ipsum quibusdam quas harum ut. Distinctio minima iusto. Ad ad maiores et sint voluptate recusandae architecto. Et nihil ullam aut alias.</div>
                            <div class="post__image">
                                <img src="../assets/images/wpengine-homepage.jpg" alt="WP Engine">
                            </div>
                            <div class="post__footer">
                                <div class="post__footer-icons">
                                    <i class="fa-regular fa-heart"></i>
                                    <i class="fa-solid fa-arrow-right-from-bracket"></i>
                                </div>
                                <div class="post__footer-time">
                                    <p>22h</p>
                                </div>
                            </div>            
                        </div>
                    </div>
                    <div class="mid-footer-contact col-3">
                        <h6>contact us today</h6>
                        <div class="contact">
                            <footer-data v-for="(item, index) in itemContact" :key="index" :icon="item.icon" :title="item.title" :address="item.address" :town="item.town"/>
                        </div>
                    </div>
                    <div class="col-3">
                        <h6>find us</h6>
                        <img src="../assets/images/2022-05-17_14-51.png" alt="Avada Location">
                    </div>
                </div>
            </div>
        </div>
        <div class="bottom-footer">
            <div class="copyright">
                <p>copyright 2012 - 2015 avada theme by <span>theme fusion</span> | all rights reserved | powered by <span>wordpress</span></p>
            </div>
            <div class="social">
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-youtube"></i>
                <i class="fa-brands fa-instagram"></i>
            </div>
            <button class="start">
                <i href="#" class="fa-solid fa-angle-up"></i>
            </button>
        </div>
    </footer>
</template>

<script>
import dati from "../contactUs.json"
import FooterData from './FooterData.vue'
export default {
    name: 'AppFooter',
    components:{
        FooterData
    },
    data(){
        return{
            itemContact: dati
        }
    }
}
</script>

<style lang="scss">
@import '../style/vars';
.top-footer{
    width: 100%;
    height: 300px;
    position: relative;
    img{
        width: 100%;
        height: 100%;
    }
    .top-footer-container{
        width: 70%;
        margin: 0 auto;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        h4{
            text-transform: capitalize;
            color: $text-color-title;
        }
        hr{
            width: 20%;
            height: 2px;
            opacity: 1;
            margin: 30px 0;
            color: $text-color-alternative;
        }
        p{
            color: $text-color-title;
        }
        button{
            @include button-layout;
            background-color: $bg-button-standard;
            color: $text-color;
        }
        .row-right p{
            color: $text-color-title;
            font-size: 10px;
            margin-top: 10px;
        }
    }
}

.mid-footer{
    background-color: $bg-footer;
    padding: 50px 0;
    .mid-footer-container{
        width: 90%;
        margin: 0 auto;
        color: $text-color;
        button{
            @include button-layout;
            background-color: $bg-button-standard;
            color: $text-color;
            margin: 0;
        }
        h6{
            text-transform: uppercase;
            color: $text-color-alternative;
            margin-bottom: 30px;
        }
        .post{
            color: $text-color-title;
            .post-meta {
                display: flex;
                justify-content: space-between;
                .post-meta__icon {
                    display: flex;
                    
                    .profile-pic {
                        border-radius: 50%;
                        max-width: 60px;
                    }
                    .post-meta__data {
                        display: flex;
                        flex-direction: column;
                        justify-content: center;
                        .post-meta__author {
                            font-weight: bold;
                        }

                        .post-meta__profile {
                            font-size: 0.8rem;
                        }
                    }
                }
                .fa-twitter{
                    color: $text-color;
                }
            }
            .post__text {
                padding-left: 50px;
            }
            .post__image {
                padding-left: 50px;
                img {
                    width: 100%;
                }
            }
            .post__footer{
                padding-left: 50px;
                display: flex;
                justify-content: space-between;
                color: $text-color;
            }
        }
        .contact{
            padding: 0 25px;
            color: $text-color;
            p i{
                margin-left: -25px;
            }
        }
    }
}

.bottom-footer{
    width: 100%;
    height: 50px;
    background-color: $bg-footer-bottom;
    color: $text-color;
    text-transform: uppercase;
    font-size: 10px;
    @include my-flex;
    padding: 0 20px;
    p{
        margin: 0;
    }
    .copyright span{
        color: $text-color-light;
    }
    .social{
        margin-right: 50px;
        font-size: 15px;
        i{
            padding-left: 10px;
        }
    }
    .start{
        position: fixed;
        bottom: 0;
        right: 5px;
        width: 40px;
        height: 25px;
        border-radius: 5px;
        background-color: $bg-button-footer;
        color: $text-color-title;
    }
}
</style>