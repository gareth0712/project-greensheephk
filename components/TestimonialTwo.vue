<template>
  <section class="pt-120 pb-110 blue-bg2">
          <div class="container">
              <div class="row justify-content-center">
                  <div class="col-8">
                      <!-- section title -->
                      <div class="section-title text-center">
                          <span class="schoolbell">Our Feedbacks</span>
                          <h2 class="text-white">Testimonials</h2>
                      </div>
                      <!-- End of section title -->
                  </div>
              </div>
              <div class="row">
                  <div class="col-12">
                      <div class="testionial-carousel-wrap type2">
                          <div class="testionial-carousel2">
                            <swiper :options="swiperOptions">
                              <swiper-slide>
                             <!-- single testimonial -->
                             <div class="single-testimonial text-center">
                                 <div class="testi-quate">
                                     <img src="/assets/img/qort-icon.png" alt="">
                                 </div>
                                 <p>There are many variations of passages of available but the majority have alteration in some form by inject humour or random words which don't look even slightly they will believe you.</p>
                                 <div class="testimonial-author">
                                     <div class="testimonial-author-deg">
                                          <h4>Kevin Martin</h4>
                                          <p>Manager</p>
                                     </div>
                                     <img src="/assets/img/team/author4.png" alt="">
                                 </div>
                             </div>
                             <!-- End of single testimonial -->
                              </swiper-slide>
                              <swiper-slide>

                             <!-- single testimonial -->
                             <div class="single-testimonial text-center">
                                 <div class="testi-quate">
                                     <img src="/assets/img/qort-icon.png" alt="">
                                 </div>
                                 <p>There are many variations of passages of available but the majority have alteration in some form by inject humour or random words which don't look even slightly they will believe you.</p>
                                 <div class="testimonial-author">
                                     <div class="testimonial-author-deg">
                                          <h4>Kevin Martin</h4>
                                          <p>Manager</p>
                                     </div>
                                     <img src="/assets/img/team/author4.png" alt="">
                                 </div>
                             </div>
                             <!-- End of single testimonial -->
                              </swiper-slide>
                              <div class="swiper-button-prev" slot="button-prev"></div>
                              <div class="swiper-button-next" slot="button-next"></div>
                            </swiper>
                          </div>
                      </div>
                  </div>
              </div>
          </div>
      </section>
</template>

<script>
  import { Swiper, SwiperSlide, directive } from 'vue-awesome-swiper';
  import 'swiper/css/swiper.css';

    export default {
      name: "TestimonialTwo",
      components: {
        Swiper,
        SwiperSlide
      },
      directives: {
        swiper: directive
      },
      data() {
        return {
          swiperOptions: {
            slidesPerView : 1,
            loop: true,
            speed: 1000,
            spaceBetween : 30,
            autoplay: {
                delay: 3000,
                disableOnInteraction: false
            },
            navigation: {
              nextEl: '.swiper-button-next',
              prevEl: '.swiper-button-prev'
            }

          }
        }
      },
    }
</script>

<style scoped>

</style>
