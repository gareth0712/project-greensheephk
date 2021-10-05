<template>
  <div class="banner-area-inner">
        <div class="banner-wrap home-banner2" style="background-image: url(/assets/img/banner/h2-banner1.png)">
          <div class="container">
            <div class="row justify-content-center">
              <div class="col-12 col-md-9">
                <!-- banner text -->
                <div class="banner-text-wrap text-center">
                  <span class="schoolbell">Order Now and Get Free Water Delivery</span>
                  <h1 class="text-white">We Deliver the Best Pure<br> Mineral Water</h1>
                </div>
                <!-- End of banner text -->
              </div>
            </div>
            <div class="row">
              <div class="col-12">
                <!-- banner form area -->
                <div class="banner-form-area">
                  <form action="#">
                    <div class="inpout-feield-wrap">
                      <input type="text" placeholder="Name" class="banner-form" required>
                      <input type="number" placeholder="Number" class="banner-form" required>
                      <input type="text" placeholder="Address" class="banner-form" required>
                      <input type="number" placeholder="Bottol" class="banner-form" required>
                      <button class="btn">Order Now</button>
                    </div>
                    <div class="form-checkbox">
                      <ul class="mb-0 list-unstyled">
                          <li>
                              <label class="checkbox-wrap">Home
                                  <input type="checkbox" name="bottol-check">
                                  <span class="checkmark"></span>
                              </label>
                          </li>
                          <li>
                              <label class="checkbox-wrap">Office
                                  <input type="checkbox" checked="checked" name="bottol-check">
                                  <span class="checkmark"></span>
                              </label>
                          </li>
                      </ul>
                  </div>
                  </form>
                </div>
                <!-- end of banner form area -->
              </div>
            </div>
          </div>
        </div>
      </div>
</template>

<script>
    export default {
      name: "BannerTwo"
    }
</script>

<style scoped>

</style>
