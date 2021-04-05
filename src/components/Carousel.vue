<template>
    <div class="car">
        <carousel :perPage="1" :autoplay="true" :autoplayTimeout="5000" :autoplayHoverPause="true" :loop="true">
            <slide>
                <div class="image">
                    <img class="images" src="../assets/1.png" alt="first">
                </div>
            </slide>
            <slide>
                <img class="images" src="../assets/2.png" alt="second">
            </slide>
            <slide>
                <img class="images" src="../assets/3.jpg" alt="third">
            </slide>
            <slide>
                <img class="images" src="../assets/4.jpg" alt="fourth">
            </slide>
        </carousel>
    </div>
</template>

<style>
    .car{
        min-height: 80%;
        min-height: 80vh;

        display: flex;
        align-items: center;

    }
    .images{
        width: 110%;
    }

    @media only screen and (min-width: 300px) and (max-width: 450px) {
        .ig-col{
            display: none;
        }
    }
</style>

<script>
import { Carousel, Slide } from 'vue-carousel';
export default {
    components: {
        Carousel,
        Slide
    }
}
</script>