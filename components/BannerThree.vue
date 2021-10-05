<template>
  <div class="banner_area1 clearfix">
          <div class="slider_overlay_area slider_height">
              <div class="container slider_height">
                  <div class="row slider_height">
                      <div class="col-md-5 offset-md-7 slider_height">
                          <!-- delivery form -->
                          <div class="banner-delivery-form">
                              <div class="form-header text-center">
                                  <h2>Delivery Form</h2>
                              </div>
                              <form action="#">
                                  <div class="row">
                                      <div class="col-lg-6">
                                          <input type="text" placeholder="Name" required class="theme-input-style">
                                      </div>
                                      <div class="col-lg-6">
                                          <input type="email" placeholder="Email" required class="theme-input-style">
                                      </div><!-- /.col -->
                                  </div><!-- /.row -->
                                  <div class="row">
                                      <div class="col-12">
                                          <input type="number" placeholder="Number" class="theme-input-style">
                                      </div><!-- /.col -->
                                  </div><!-- /.row -->
                                  <div class="row">
                                      <div class="col-12">
                                          <input type="text" placeholder="Address" class="theme-input-style">
                                      </div><!-- /.col -->
                                  </div><!-- /.row -->
                                  <div class="row">
                                      <div class="col-12">
                                          <input type="text" placeholder="Choose Bottles" class="theme-input-style">
                                      </div><!-- /.col -->
                                  </div><!-- /.row -->
                                  <div class="row">
                                      <div class="col">
                                          <div class="form-checkbox type2">
                                              <ul class="mb-0 list-unstyled">
                                                  <li>
                                                      <label class="checkbox-wrap">Home
                                                          <input type="checkbox">
                                                          <span class="checkmark"></span>
                                                      </label>
                                                  </li>
                                                  <li>
                                                      <label class="checkbox-wrap">Office
                                                          <input type="checkbox" checked="checked">
                                                          <span class="checkmark"></span>
                                                      </label>
                                                  </li>
                                              </ul>
                                          </div>
                                      </div><!-- /.col -->
                                  </div><!-- /.row -->
                                  <div class="row">
                                      <div class="col">
                                          <div class="form-btn">
                                              <button class="btn" type="submit">Order Now</button>
                                          </div>
                                      </div><!-- /.col -->
                                  </div><!-- /.row -->
                              </form><!-- /.form -->
                          </div><!-- End of delivery form -->
                      </div><!-- /.col -->
                  </div><!-- /.row -->
              </div><!-- /.container -->
          </div><!-- /.overlay -->
          <div class="camera_wrap " id="banner_slider1">
              <div class="hero_slider" style="background-image: url(/assets/img/banner/h3-banner2.jpg); background-size: cover;height: 770px;">
                  <div class="container">
                      <div class="row">
                          <div class="col-md-7">
                              <!-- banner text wrap -->
                              <div class="banner-text-wrap">
                                  <span class="schoolbell fadeInUp">Enjoy great tasting bottled water</span>
                                  <h1 class="text-white fadeInUp">We deliver the<br> best pure mineral water</h1>
                                  <a href="#" class="btn fadeInUp">Order Now</a>
                              </div><!--/.End of  banner text wrap -->
                          </div><!-- /.col -->
                      </div><!-- /.row -->
                  </div><!--/.container-->
              </div><!--/.Slider Item-->
          </div><!-- /.camera wrap -->
      </div>
</template>

<script>
    export default {
        name: "BannerThree"
    }
</script>

<style scoped>

</style>
