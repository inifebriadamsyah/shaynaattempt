<script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide, Pagination, Navigation } from "vue3-carousel";

export default {
    name: "HeroShayna",
    components: {
        Carousel,
        Slide,
        Pagination,
        Navigation,
    },
};
</script>

<style scoped>
.set-bg {
    width: 100%;
    height: 720px;
}

.banner-info {
    margin-top: 220px;
}
</style>

<template>
    <div>
        <!-- Hero Section Begin -->
        <section class="hero-section">
            <carousel :items-to-show="1" :autoplay="1500" :wrap-around="true">
                <slide v-for="slide in 1" :key="slide">
                    <div class="single-hero-items set-bg" style="background-image: url('/img/hero-1.jpg')">
                        <div class="container">
                            <div class="row banner-info">
                                <div class="col-lg-5">
                                    <span
                                        style="color: #e7ab3c;  text-transform: uppercase;  font-weight: 700; letter-spacing: 3px;">Bag,
                                        kids</span>
                                    <h1 style="font-weight: 700">Black friday</h1>
                                    <p style="margin-top: 12px; margin-bottom: 20px; font-size: 16px">
                                        Lorem ipsum dolor sit amet, consectetur adipisicing elit,
                                        sed do eiusmod tempor incididunt ut labore et dolore
                                    </p>
                                    <a href="#" class="primary-btn">Shop Now</a>
                                </div>
                            </div>
                        </div>
                    </div>
                </slide>
                <slide v-for="slide in 1" :key="slide">
                    <div class="single-hero-items set-bg" style="background-image: url('/img/hero-2.jpg')">
                        <div class="container">
                            <div class="row banner-info">
                                <div class="col-lg-5">
                                    <span
                                        style="color: #e7ab3c;  text-transform: uppercase;  font-weight: 700; letter-spacing: 3px;">Bag,
                                        kids</span>
                                    <h1 style="font-weight: 700">Black friday</h1>
                                    <p style="margin-top: 12px; margin-bottom: 20px; font-size: 16px">
                                        Lorem ipsum dolor sit amet, consectetur adipisicing elit,
                                        sed do eiusmod tempor incididunt ut labore et dolore
                                    </p>
                                    <a href="#" class="primary-btn">Shop Now</a>
                                </div>
                            </div>
                        </div>
                    </div>
                </slide>
                <slide v-for="slide in 1" :key="slide">
                    <div class="single-hero-items set-bg" style="background-image: url('/img/hero-3.jpg')">
                        <div class="container">
                            <div class="row banner-info">
                                <div class="col-lg-5">
                                    <span
                                        style="color: #e7ab3c;  text-transform: uppercase;  font-weight: 700; letter-spacing: 3px;">Bag,
                                        kids</span>
                                    <h1 style="font-weight: 700">Black friday</h1>
                                    <p style="margin-top: 12px; margin-bottom: 20px; font-size: 16px">
                                        Lorem ipsum dolor sit amet, consectetur adipisicing elit,
                                        sed do eiusmod tempor incididunt ut labore et dolore
                                    </p>
                                    <a href="#" class="primary-btn">Shop Now</a>
                                </div>
                            </div>
                        </div>
                    </div>
                </slide>

                <template #addons>
                    <navigation />
                    <pagination />
                </template>
            </carousel>
        </section>
    <!-- Hero Section End -->
</div></template>