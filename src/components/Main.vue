<template>
    <div>
        <b-container class="container">
            <b-row class="row">
                <b-col></b-col>
                <b-col class="col" align-self="center">
                    <img src="../assets/logo.png" alt="logo">
                </b-col>
                <b-col class="ig-col" align-self="end"> 
                    <a target="blank" href="https://www.instagram.com/complementario.mx/">
                        <img class="ig-logo" src="../assets/instagram.png" alt="ig">
                    </a>
                </b-col>
            </b-row>
        </b-container>

        <b-container>
            <b-row>
                <b-col>
                    <h1 align-self="center" class="coming-soon">coming soon</h1>
                </b-col>
            </b-row>
        </b-container>

        <b-container>
            <b-row>
                <b-col>
                    <Carousel />
                </b-col>
            </b-row>
        </b-container>
        
    </div>
</template>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital@1&display=swap');
    .coming-soon{
        font-size: 32px;
        font-family: 'Playfair Display', serif;
    }
    .ig-col{
        margin: auto;
    }
    .coming-soon{
        margin: 0 auto;
    }
    .ig-logo{
        width: 15%;
        float: right;
    }

    @media only screen and (min-width: 300px) and (max-width: 450px) {
        .ig-col{
            display: none;
        }
    }
</style>

<script>
import Carousel from './Carousel.vue'
export default {
    components: {
        Carousel
    }
}
</script>