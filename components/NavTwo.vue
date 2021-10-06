<template>
  <header class="header">
          <!-- Start Header Navbar-->
          <div :class="`main-header header-style2 ${sticky ? 'sticky fadeInDown' : ''}`">
              <div class="main-menu-wrap">
                  <div class="container-fluide">
                      <div class="row align-items-center">
                          <div class="col-xl-3 col-lg-3 col-md-4 col-sm-4 col-6">
                              <!-- Logo -->
                              <div class="logo">
                                  <nuxt-link to="/">
                                      <img class="main-logo" src="/assets/img/logo2.png" data-rjs="2" alt="mineralo">
                                      <img class="sticky-logo d-none" src="/assets/img/logo.png" data-rjs="2" alt="mineralo">
                                  </nuxt-link>
                              </div>
                              <!-- End of Logo -->
                          </div>
                          <div class="col-xl-6 col-lg-6 col-md-4 col-sm-4 col-6 menu-button">
                              <div class="menu--inner-area clearfix">
                                  <div class="menu-wraper">
                                      <nav>
                                          <!-- Header-menu -->
                                          <div class="header-menu dosis">
                                            <div @click="mobileToggle = !mobileToggle" id="menu-button" class=""><i class="fa fa-bars"></i></div>
                                              <ul>
                                                  <li class="active"><nuxt-link to="/">Home <img src="/assets/img/line2.png" alt=""></nuxt-link>
                                                      <ul>
                                                        <li class="active"><nuxt-link to="/">Home v1</nuxt-link></li>
                                                        <li><nuxt-link to="/index-2">Home v2</nuxt-link></li>
                                                        <li><nuxt-link to="/index-3">Home v3</nuxt-link></li>
                                                      </ul>
                                                  </li>
                                                <li><nuxt-link to="/about">About <img src="/assets/img/line2.png" alt=""></nuxt-link></li>
                                                <li><nuxt-link to="#">Service<img src="/assets/img/line2.png" alt=""></nuxt-link>
                                                    <ul>
                                                        <li><nuxt-link to="/service">Service</nuxt-link></li>
                                                        <li><nuxt-link to="/service-details">Service Details</nuxt-link></li>
                                                    </ul>
                                                </li>
                                                <li>
                                                    <nuxt-link to="#">Blog <img src="/assets/img/line2.png" alt=""></nuxt-link>
                                                    <ul>
                                                        <li><nuxt-link to="/blog">Blog Layout</nuxt-link></li>
                                                        <li><nuxt-link to="/blog-details">Blog Details</nuxt-link></li>
                                                    </ul>
                                                </li>
                                                <li><nuxt-link to="/contact">Contact<img src="/assets/img/line2.png" alt=""></nuxt-link></li>
                                              </ul>
                                          </div>
                                          <!-- End of Header-menu -->
                                      </nav>
                                  </div>
                              </div>
                          </div>
                          <div class="col-lg-3 col-md-4 col-sm-4">
                              <div class="urgent-call text-right">
                                  <span><img src="/assets/img/icons/call.svg" class="svg" alt="Contact Number"></span><a href="#" @click="openBrowser(whatsappLink)">+852 5440 7482</a>
                              </div>
                          </div>
                        <div class="mobile-nav">
                          <ul :style="`display: ${mobileToggle ? 'block' : 'none'}`" class="open">
                            <li class="active has-sub-item"><span class="submenu-button submenu-opened"></span><a href="#">Home</a>
                              <ul>
                                <li class="active"><nuxt-link to="/">Home v1</nuxt-link></li>
                                <li><nuxt-link to="/index-2">Home v2</nuxt-link></li>
                                <li><nuxt-link to="/index-3">Home v3</nuxt-link></li>
                              </ul>
                            </li>
                            <li><nuxt-link to="/about">About</nuxt-link></li>
                            <li class="has-sub-item"><span class="submenu-button"></span><a href="#">Service</a>
                              <ul>
                                <li><nuxt-link to="/service">Service</nuxt-link></li>
                                <li><nuxt-link to="/service-details">Service Details</nuxt-link></li>
                              </ul>
                            </li>
                            <li class="has-sub-item"><span class="submenu-button"></span>
                              <a href="#">Blog</a>
                              <ul>
                                <li><nuxt-link to="/blog">Blog Layout</nuxt-link></li>
                                <li><nuxt-link to="/blog-details">Blog Details</nuxt-link></li>
                              </ul>
                            </li>
                            <li><nuxt-link to="/contact">Contact</nuxt-link></li>
                          </ul>
                        </div>
                      </div>
                  </div>
              </div>
          </div>
          <!-- End Header Navbar-->
      </header>
</template>

<script>
    export default {
      name: "NavTwo",
      data(){
        return {
          sticky: false,
          mobileToggle: false,
          whatsappLink: 'https://api.whatsapp.com/send?phone=85254407482&app=facebook&entry_point=page_cta&fbclid=IwAR155hKk6PZq-9X0jaivk57VMwjiRSJCj02Ej2IhHozW_Pkr2X9oVf56gM8'
        }
      },
      mounted() {
        window.addEventListener('scroll', this.handleScroll);
      },
      methods: {
        openBrowser(link) {
          if (!link) return;
          window.open(link);
        },
        handleScroll() {
          if (window.scrollY > 70) {
            this.sticky = true
          } else if (window.scrollY < 70) {
            this.sticky = false
          }
        },
      }
    }
</script>

<style scoped>

</style>
