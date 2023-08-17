<template>
  <div class="home">
    <HeaderShayna />

    <!-- Breadcrumb Section Begin -->
    <div class="breacrumb-section text-left">
      <div class="container">
        <div class="row">
          <div class="col-lg-12">
            <div class="breadcrumb-text product-more">
              <router-link to="/">
                <i class="fa fa-home"></i> Home
              </router-link>
              <span>Detail</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- Breadcrumb Section Begin -->

    <!-- Product Shop Section Begin -->
    <section class="product-shop spad page-details">
      <div class="container">
        <div class="row">
          <div class="col-lg-12">
            <div class="row">
              <div class="col-lg-6">
                <div class="product-pic-zoom px-2 mb-4">
                  <img class="product-big-img" :src="pict_default" alt="" />
                </div>
                <div class="product-thumbs px-0">
                  <Carousel :itemsToShow="3" v-bind="settings" :breakpoints="breakpoints">
                    <Slide v-for="slide in 1" :key="slide">
                      <div class="carousel__item">
                        <div class="carousel__item mx-2">
                          <div @click="changeImage(thumbs[0])" class="pt" :class="thumbs[0] == pict_default ? 'active' : '' ">
                            <img src="img/mickey1.jpg" alt="" />
                          </div>
                        </div>
                      </div>
                    </Slide>
                    <Slide v-for="slide in 1" :key="slide">
                      <div class="carousel__item">
                        <div class="carousel__item mx-2">
                          <div @click="changeImage(thumbs[1])" class="pt" :class="thumbs[1] == pict_default ? 'active' : '' ">
                            <img src="img/mickey2.jpg" alt="" />
                          </div>
                        </div>
                      </div>
                    </Slide>
                    <Slide v-for="slide in 1" :key="slide">
                      <div class="carousel__item">
                        <div class="carousel__item mx-2">
                          <div @click="changeImage(thumbs[2])" class="pt" :class="thumbs[2] == pict_default ? 'active' : '' ">
                            <img src="img/mickey3.jpg" alt="" />
                          </div>
                        </div>
                      </div>
                    </Slide>
                    <Slide v-for="slide in 1" :key="slide">
                      <div class="carousel__item">
                        <div class="carousel__item mx-2">
                          <div @click="changeImage(thumbs[3])" class="pt" :class="thumbs[3] == pict_default ? 'active' : '' ">
                            <img src="img/mickey4.jpg" alt="" />
                          </div>
                        </div>
                      </div>
                    </Slide>

                    <template #addons>
                      <Navigation />
                    </template>
                  </Carousel>
                </div>
                <!--
                <div class="product-thumbs">
                  <Carousel id="gallery" :items-to-show="1" :wrap-around="false" v-model="currentSlide">
                    <Slide v-for="slide in 4" :key="slide">
                      <div class="carousel__item">
                        <div class="product-pic-zoom">
                          <img class="product-big-img" src="img/mickey1.jpg" alt="" />
                        </div>
                      </div>
                    </Slide>
                  </Carousel>
                  <Carousel
                      id="thumbnails"
                      :items-to-show="3"
                      :wrap-around="true"
                      v-model="currentSlide"
                      ref="carousel"
                      class="my-4"
                      style="padding: 0px 60px;"
                    >
                    <Slide v-for="slide in 1" :key="slide">
                        <div class="carousel__item mx-2" @click="slideTo(slide - 1)">
                          <div data-imgbigurl="img/mickey1.jpg">
                            <img src="img/mickey1.jpg" alt="" />
                          </div>
                        </div>
                      </Slide>
                      <Slide v-for="slide in 1" :key="slide">
                        <div class="carousel__item mx-2" @click="slideTo(slide - 1)">
                          <div class="" data-imgbigurl="img/mickey2.jpg">
                            <img src="img/mickey2.jpg" alt="" />
                          </div>
                        </div>
                      </Slide>
                      <Slide v-for="slide in 1" :key="slide">
                        <div class="carousel__item mx-2" @click="slideTo(slide - 1)">
                          <div class="" data-imgbigurl="img/mickey3.jpg">
                            <img src="img/mickey3.jpg" alt="" />
                          </div>
                        </div>
                      </Slide>
                      <Slide v-for="slide in 1" :key="slide">
                        <div class="carousel__item mx-2" @click="slideTo(slide - 1)">
                          <div class="pt active" data-imgbigurl="img/mickey4.jpg">
                            <img src="img/mickey4.jpg" alt="" />
                          </div>
                        </div>
                      </Slide>
                    </Carousel>
                </div>
                  -->
              </div>
              <div class="col-lg-6">
                <div class="product-details text-left">
                  <div class="pd-title">
                    <span>oranges</span>
                    <h3>Pure Pineapple</h3>
                  </div>
                  <div class="pd-desc">
                    <p>
                      Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis, error officia. Rem aperiam
                      laborum voluptatum vel, pariatur modi hic provident eum iure natus quos non a sequi, id accusantium!
                      Autem.
                    </p>
                    <p>
                      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quam possimus quisquam animi, commodi,
                      nihil voluptate nostrum neque architecto illo officiis doloremque et corrupti cupiditate
                      voluptatibus error illum. Commodi expedita animi nulla aspernatur.
                      Id asperiores blanditiis, omnis repudiandae iste inventore cum, quam sint molestiae accusamus
                      voluptates ex tempora illum sit perspiciatis. Nostrum dolor tenetur amet, illo natus magni veniam
                      quia sit nihil dolores.
                      Commodi ratione distinctio harum voluptatum velit facilis voluptas animi non laudantium, id dolorem
                      atque perferendis enim ducimus? A exercitationem recusandae aliquam quod. Itaque inventore
                      obcaecati, unde quam
                      impedit praesentium veritatis quis beatae ea atque perferendis voluptates velit architecto?
                    </p>
                    <h4>$495.00</h4>
                  </div>
                  <div class="quantity">
                    <router-link to="/cart">
                      <a href="#" class="primary-btn pd-cart">Add To Cart</a>
                    </router-link>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Product Shop Section End -->

    <RelatedProductShayna />
    <FooterShayna />
  </div>
</template>

<script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide } from "vue3-carousel";

import HeaderShayna from "@/components/HeaderShayna.vue";
import RelatedProductShayna from "@/components/RelatedProductShayna.vue";
import FooterShayna from "@/components/FooterShayna.vue";

export default {
  name: "ProductView",
  components: {
    HeaderShayna,
    RelatedProductShayna,
    FooterShayna,
    Carousel,
    Slide
  },
  props: {
    msg: String,
  },
  /*
  data: () => ({
    currentSlide: 0,
  }),
  methods: {
    slideTo(val) {
      this.currentSlide = val
    },
  },
  */
  data2: () => ({
    // carousel settings
    settings: {
      itemsToShow: 4,
      snapAlign: 'center',
    },
    // breakpoints are mobile first
    // any settings not specified will fallback to the carousel settings
    breakpoints: {
      // 700px and up
      500: {
        itemsToShow: 4.5,
        snapAlign: 'center',
      },
      // 1024 and up
      1024: {
        itemsToShow: 3,
        snapAlign: 'start',
      },
    },
  }),

  data() {
    return {
      pict_default: "img/mickey1.jpg",
      thumbs: [
        "img/mickey1.jpg",
        "img/mickey2.jpg",
        "img/mickey3.jpg",
        "img/mickey4.jpg"
      ]
    }
  },

  methods: {
    changeImage(urlImage) {
      this.pict_default = urlImage;
    }
  },
};
</script>

  <!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
