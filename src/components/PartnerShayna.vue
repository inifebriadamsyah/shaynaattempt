<script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide } from "vue3-carousel";

export default {
    name: 'PartnerShayna',
    components: {
        Carousel,
        Slide
    },
}
</script>
<style scoped>
/* Create two equal columns that floats next to each other */
.column {
    float: left;
    text-align: center;
    align-items: center;
    width: 20%;
    padding: 32px;
    height: 100px;
    /* Should be removed. Only for demonstration */
}

/* Clear floats after the columns */
.row:after {
    content: "";
    display: table;
    clear: both;
    align-items: center;
}
</style>
<template>

    <!-- Partner Logo Section Begin -->
    <!--
    <div class="partner-logo">
        <div class="container">
            <div class="logo-carousel owl-carousel">
                <div class="logo-item">
                    <div class="tablecell-inner">
                        <img src="img/logo-carousel/logo-1.png" alt="" />
                    </div>
                </div>
                <div class="logo-item">
                    <div class="tablecell-inner">
                        <img src="img/logo-carousel/logo-2.png" alt="" />
                    </div>
                </div>
                <div class="logo-item">
                    <div class="tablecell-inner">
                        <img src="img/logo-carousel/logo-3.png" alt="" />
                    </div>
                </div>
                <div class="logo-item">
                    <div class="tablecell-inner">
                        <img src="img/logo-carousel/logo-4.png" alt="" />
                    </div>
                </div>
                <div class="logo-item">
                    <div class="tablecell-inner">
                        <img src="img/logo-carousel/logo-5.png" alt="" />
                    </div>
                </div>
            </div>
        </div>
    </div>
    -->
    <!-- Partner Logo Section End -->


    <div class="partner-logo">
        <div class="container" style="align-items:center">
            <Carousel :items-to-show="5" :wrap-around="true" :autoplay="2500">
                <Slide v-for="slide in 1" :key="slide">
                    <div class="carousel__item">
                        <div>
                            <div class="logo-item ">
                                <div class="tablecell-inner">
                                    <img src="img/logo-carousel/logo-1.png" alt="" />
                                </div>
                            </div>
                        </div>
                    </div>
                </Slide>
                <Slide v-for="slide in 1" :key="slide">
                    <div class="carousel__item">
                        <div>
                            <div class="logo-item ">
                                <div class="tablecell-inner">
                                    <img src="img/logo-carousel/logo-2.png" alt="" />
                                </div>
                            </div>
                        </div>
                    </div>
                </Slide>
                <Slide v-for="slide in 1" :key="slide">
                    <div class="carousel__item">
                        <div>
                            <div class="logo-item ">
                                <div class="tablecell-inner">
                                    <img src="img/logo-carousel/logo-3.png" alt="" />
                                </div>
                            </div>
                        </div>
                    </div>
                </Slide>
                <Slide v-for="slide in 1" :key="slide">
                    <div class="carousel__item">
                        <div>
                            <div class="logo-item ">
                                <div class="tablecell-inner">
                                    <img src="img/logo-carousel/logo-4.png" alt="" />
                                </div>
                            </div>
                        </div>
                    </div>
                </Slide>
                <Slide v-for="slide in 1" :key="slide">
                    <div class="carousel__item">
                        <div>
                            <div class="logo-item ">
                                <div class="tablecell-inner">
                                    <img src="img/logo-carousel/logo-5.png" alt="" />
                                </div>
                            </div>
                        </div>
                    </div>
                </Slide>

                <template #addons>

                </template>
            </Carousel>

        </div>
    </div>

    <!-- Partner Logo Section End -->
</template>