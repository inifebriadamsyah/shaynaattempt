<script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide, Navigation } from "vue3-carousel";

export default {
    name: "WomenBannerShayna",
    components: {
        Carousel,
        Slide,
        Navigation
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
    <div style="margin-top: 32px; margin-bottom: 44px">
        <!-- Women Banner Section Begin -->
        <section class="women-banner spad">
            <div class="container-fluid">
                <div class="row d-flex justify-content-center">
                    <div class="col-lg-10 mt-5">
                        <Carousel :items-to-show="3.75" :wrap-around="true" >
                            <Slide v-for="slide in 1" :key="slide">
                                <div class="carousel__item">
                                    <div class="product-item">
                                        <div class="pi-pic">
                                            <img src="img/products/women-1.jpg" style="height:440px" alt="" />
                                            <ul>
                                                <li class="w-icon active">
                                                    <a href="#"><i class="icon_bag_alt"></i></a>
                                                </li>
                                                <li class="quick-view"><router-link to="/product">+ Quick View</router-link></li>
                                            </ul>
                                        </div>
                                        <div class="pi-text">
                                            <div class="catagory-name">Coat</div>
                                            <router-link to="/">
                                                <h5>Shanghai sweater</h5>
                                            </router-link>
                                            <div class="product-price">
                                                $14.00
                                                <span>$35.00</span>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </Slide>
                            <Slide v-for="slide in 1" :key="slide">
                                <div class="carousel__item">
                                    <div class="product-item">
                                        <div class="pi-pic">
                                            <img src="img/products/women-2.jpg" style="height:440px" alt="" />
                                            <ul>
                                                <li class="w-icon active">
                                                    <a href="#"><i class="icon_bag_alt"></i></a>
                                                </li>
                                                <li class="quick-view"><a href="#">+ Quick View</a></li>
                                            </ul>
                                        </div>
                                        <div class="pi-text">
                                            <div class="catagory-name">Shoes</div>
                                            <a href="#">
                                                <h5>Guangzhou sweater</h5>
                                            </a>
                                            <div class="product-price">
                                                $13.00
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </Slide>
                            <Slide v-for="slide in 1" :key="slide">
                                <div class="carousel__item">
                                    <div class="product-item">
                                        <div class="pi-pic">
                                            <img src="img/products/women-3.jpg" style="height:440px" alt="" />
                                            <ul>
                                                <li class="w-icon active">
                                                    <a href="#"><i class="icon_bag_alt"></i></a>
                                                </li>
                                                <li class="quick-view"><a href="#">+ Quick View</a></li>
                                            </ul>
                                        </div>
                                        <div class="pi-text">
                                            <div class="catagory-name">Towel</div>
                                            <a href="#">
                                                <h5>Pure Pineapple</h5>
                                            </a>
                                            <div class="product-price">
                                                $34.00
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </Slide>
                            <Slide v-for="slide in 1" :key="slide">
                                <div class="carousel__item">
                                    <div class="product-item">
                                        <div class="pi-pic">
                                            <img src="img/products/women-4.jpg"  style="height:440px" alt="" />
                                            <ul>
                                                <li class="w-icon active">
                                                    <a href="#"><i class="icon_bag_alt"></i></a>
                                                </li>
                                                <li class="quick-view"><a href="#">+ Quick View</a></li>
                                                <li class="w-icon">
                                                    <a href="#"><i class="fa fa-random"></i></a>
                                                </li>
                                            </ul>
                                        </div>
                                        <div class="pi-text">
                                            <div class="catagory-name">Towel</div>
                                            <a href="#">
                                                <h5>Converse Shoes</h5>
                                            </a>
                                            <div class="product-price">
                                                $34.00
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </Slide>

                            <template #addons>
                                <Navigation />

                            </template>
                        </Carousel>
                        <div class="product-slider owl-carousel">




                        </div>
                    </div>
                </div>
            </div>
        </section>
        <!-- Women Banner Section End -->
    </div>
</template>