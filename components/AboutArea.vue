<template>
  <section class="pt-120 pb-120 primary-bg">
         <div class="container">
             <div class="row align-items-center">
                 <div class="col-lg-6">
                     <div class="about-image">
                         <img src="/assets/img/about-img.png" alt="">
                     </div>
                 </div>
                 <div class="col-lg-6">
                     <!-- about inner -->
                     <div class="about-wrap">
                         <!-- section title -->
                          <div class="section-title type2">
                              <span class="schoolbell">Shortly About Us</span>
                              <h2>Learn About Mineralo</h2>
                          </div>
                         <!-- End of section title -->
                         <div class="about-area-text">
                             <p>There are many variations of passages of available but the majority have alteration in some form by inject humour or random words which don't look even slightly they will believe you. proident.</p>
                             <div v-observe-visibility="onVisibilityChange" class="about-counter-inner">
                                 <div class="row">
                                     <div class="col-12 col-sm-6">
                                         <!-- single counter -->
                                         <div class="single-counter-inner text-center">
                                             <div class="counter-image">
                                                 <img src="/assets/img/icons/water-bottle(2).svg" class="svg" alt="">
                                             </div>
                                             <span class="counter">
                                               <countTo :startVal='0' :endVal='startCounter ? 6780 : 0' :duration='3000'></countTo>
                                             </span>
                                             <p>Bottles Delivered</p>
                                         </div>
                                         <!-- End of single counter -->
                                     </div>
                                     <div class="col-12 col-sm-6">
                                         <!-- single counter -->
                                         <div class="single-counter-inner text-center">
                                             <div class="counter-image">
                                                 <img src="/assets/img/icons/water-bottle(1).svg" class="svg" alt="">
                                             </div>
                                             <span class="counter">
                                               <countTo :startVal='0' :endVal='startCounter ? 8430 : 0' :duration='3000'></countTo>
                                             </span>
                                             <p>Satisfied Customer</p>
                                         </div>
                                         <!-- End of single counter -->
                                     </div>
                                 </div>
                             </div>
                         </div>
                     </div>
                     <!-- End of about inner -->
                 </div>
             </div>
         </div>
      </section>
</template>

<script>
  import countTo from 'vue-count-to';
  import { ObserveVisibility } from 'vue-observe-visibility'

    export default {
      name: "AboutArea",
      components: { countTo },
      directives: {
        ObserveVisibility
      },
      data() {
        return{
          startCounter: false
        }
      },
      methods: {
        onVisibilityChange (isVisible) {
          if (isVisible){
            this.startCounter = true;
          }

        },
      },

    }
</script>

<style scoped>

</style>
