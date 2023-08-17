<script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide } from "vue3-carousel";

export default {
    name: "RelatedProductShayna",
    components: {
        Carousel,
        Slide
    },
};
</script>

<template>

     <!-- Related Products Section End -->
     <div class="related-products spad mt-5">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="section-title">
                        <h2>Related Products</h2>
                    </div>
                </div>
            </div>
            <div class="row">
                <Carousel :items-to-show="4" :wrap-around="false">
                    <Slide v-for="slide in 1" :key="slide" class="mx-1">
                        <div class="carousel__item">
                            <div class="product-item">
                                <div class="pi-pic">
                                    <img src="img/products/women-2.jpg" alt="" />
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
                    <Slide v-for="slide in 1" :key="slide" class="mx-1">
                        <div class="carousel__item">
                            <div class="product-item">
                                <div class="pi-pic">
                                    <img src="img/products/women-3.jpg" alt="" />
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
                    <Slide v-for="slide in 1" :key="slide" class="mx-1">
                        <div class="carousel__item">
                            <div class="product-item">
                                <div class="pi-pic">
                                    <img src="img/products/women-1.jpg" alt="" />
                                    <ul>
                                        <li class="w-icon active">
                                            <a href="#"><i class="icon_bag_alt"></i></a>
                                        </li>
                                        <li class="quick-view"><a href="#">+ Quick View</a></li>
                                    </ul>
                                </div>
                                <div class="pi-text">
                                    <div class="catagory-name">Coat</div>
                                    <a href="#">
                                        <h5>Pure Pineapple</h5>
                                    </a>
                                    <div class="product-price">
                                        $14.00
                                        <span>$35.00</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </Slide>
                    <Slide v-for="slide in 1" :key="slide" class="mx-1">
                        <div class="carousel__item">
                            <div class="product-item">
                                <div class="pi-pic">
                                    <img src="img/products/women-4.jpg" alt="" />
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
                                        <h5>Converse Shoes</h5>
                                    </a>
                                    <div class="product-price">
                                        $34.00
                                    </div>
                                </div>
                            </div>
                        </div>
                    </Slide>
                    <Slide v-for="slide in 1" :key="slide" class="mx-1">
                        <div class="carousel__item">
                            <div class="product-item">
                                <div class="pi-pic">
                                    <img src="img/products/women-2.jpg" alt="" />
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
                    <Slide v-for="slide in 1" :key="slide" class="mx-1">
                        <div class="carousel__item">
                            <div class="product-item">
                                <div class="pi-pic">
                                    <img src="img/products/women-3.jpg" alt="" />
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
                    <Slide v-for="slide in 1" :key="slide" class="mx-1">
                        <div class="carousel__item">
                            <div class="product-item">
                                <div class="pi-pic">
                                    <img src="img/products/women-1.jpg" alt="" />
                                    <ul>
                                        <li class="w-icon active">
                                            <a href="#"><i class="icon_bag_alt"></i></a>
                                        </li>
                                        <li class="quick-view"><a href="#">+ Quick View</a></li>
                                    </ul>
                                </div>
                                <div class="pi-text">
                                    <div class="catagory-name">Coat</div>
                                    <a href="#">
                                        <h5>Pure Pineapple</h5>
                                    </a>
                                    <div class="product-price">
                                        $14.00
                                        <span>$35.00</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </Slide>
                    <Slide v-for="slide in 1" :key="slide" class="mx-1">
                        <div class="carousel__item">
                            <div class="product-item">
                                <div class="pi-pic">
                                    <img src="img/products/women-4.jpg" alt="" />
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
                                        <h5>Converse Shoes</h5>
                                    </a>
                                    <div class="product-price">
                                        $34.00
                                    </div>
                                </div>
                            </div>
                        </div>
                    </Slide>
                </Carousel>
            </div>
        </div>
    </div>
    <!-- Related Products Section End -->
</template>
