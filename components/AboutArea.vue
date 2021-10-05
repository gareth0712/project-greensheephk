<template>
  <section class="pt-120 pb-120 primary-bg">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-6">
          <div class="about-image">
            <img src="/assets/img/about-img.png" alt="" />
          </div>
        </div>
        <div class="col-lg-6">
          <!-- about inner -->
          <div class="about-wrap">
            <!-- section title -->
            <div class="section-title type2">
              <span class="schoolbell">關於我們</span>
              <h2>了解懶羊羊更多</h2>
            </div>
            <!-- End of section title -->
            <div class="about-area-text">
              <p>
                一家四口中產家庭將「懶洋洋達到財務自由」為終極目標，將有限資金作有效配置，秒秒鐘躺著收錢！懶羊羊爸爸汲取投資失利的教訓，做好風險管理，穩健增值財富！
              </p>
              <div
                v-observe-visibility="onVisibilityChange"
                class="about-counter-inner"
              >
                <div class="row">
                  <div class="col-12 col-sm-6">
                    <!-- single counter -->
                    <div class="single-counter-inner text-center">
                      <div class="counter-image">
                        <img
                          src="/assets/img/icons/water-bottle(2).svg"
                          class="svg"
                          alt=""
                        />
                      </div>
                      <span class="counter">
                        <countTo
                          :startVal="0"
                          :endVal="startCounter ? 6780 : 0"
                          :duration="3000"
                        ></countTo>
                      </span>
                      <p>Bottles Delivered</p>
                    </div>
                    <!-- End of single counter -->
                  </div>
                  <div class="col-12 col-sm-6">
                    <!-- single counter -->
                    <div class="single-counter-inner text-center">
                      <div class="counter-image">
                        <img
                          src="/assets/img/icons/water-bottle(1).svg"
                          class="svg"
                          alt=""
                        />
                      </div>
                      <span class="counter">
                        <countTo
                          :startVal="0"
                          :endVal="startCounter ? 8430 : 0"
                          :duration="3000"
                        ></countTo>
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
import { ObserveVisibility } from 'vue-observe-visibility';

export default {
  name: 'AboutArea',
  components: { countTo },
  directives: {
    ObserveVisibility,
  },
  data() {
    return {
      startCounter: false,
    };
  },
  methods: {
    onVisibilityChange(isVisible) {
      if (isVisible) {
        this.startCounter = true;
      }
    },
  },
};
</script>

<style scoped></style>
