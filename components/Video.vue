<template>
  <section class="pt-120 background-shap">
          <div class="container">
              <div class="row justify-content-center">
                  <div class="col-12">
                      <!-- section title -->
                      <div class="section-title text-center">
                          <span class="schoolbell">Watch Our Video</span>
                          <h2>Why Bottled Water?</h2>
                      </div>
                      <!-- End of section title -->
                  </div>
              </div>
              <div class="row">
                  <div class="col-12">
                      <!-- why bottle video -->
                      <div class="bottle-video-wrap">
                          <img src='/assets/img/video-bg.jpg' alt="">
                          <a href="https://www.youtube.com/watch?v=SZEflIVnhH8" class="video-btn mediabox" data-popup="video"><i class="fa fa-play"></i></a>
                      </div>
                      <!-- end of why bottle video -->
                  </div>
              </div>
          </div>
      </section>
</template>

<script>
    export default {
      name: "Video",
      mounted() {
        MediaBox('.mediabox');
      }


    }
</script>

<style scoped>

</style>
