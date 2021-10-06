<template>
  <header class="header">
    <!-- Start Header Navbar-->
    <div
      :class="`main-header header-style2 ${sticky ? 'sticky fadeInDown' : ''}`"
    >
      <div class="main-menu-wrap">
        <div class="container-fluide">
          <div class="row align-items-center">
            <div class="col-xl-3 col-lg-3 col-md-4 col-sm-4 col-6">
              <!-- Logo -->
              <div class="logo">
                <nuxt-link to="/">
                  <img
                    class="main-logo"
                    src="/logo.png"
                    data-rjs="2"
                    alt="Money Sheep"
                  />
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
                      <div
                        @click="mobileToggle = !mobileToggle"
                        id="menu-button"
                        class=""
                      >
                        <i class="fa fa-bars"></i>
                      </div>
                      <ul>
                        <li class="active">
                          <nuxt-link to="#Banner"
                            >主頁<img src="/assets/img/line2.png" alt=""
                          /></nuxt-link>
                        </li>
                        <li>
                          <nuxt-link to="#About"
                            >關於我們 <img src="/assets/img/line2.png" alt=""
                          /></nuxt-link>
                        </li>
                        <li>
                          <nuxt-link to="#Blog"
                            >Blog <img src="/assets/img/line2.png" alt=""
                          /></nuxt-link>
                        </li>
                        <li>
                          <nuxt-link to="#Contact"
                            >聯絡我們<img src="/assets/img/line2.png" alt=""
                          /></nuxt-link>
                        </li>
                      </ul>
                    </div>
                    <!-- End of Header-menu -->
                  </nav>
                </div>
              </div>
            </div>
            <div class="col-lg-3 col-md-4 col-sm-4">
              <div class="urgent-call text-right">
                <span
                  ><img
                    src="/assets/img/icons/call.svg"
                    class="svg"
                    alt="Contact Number"/></span
                ><a href="#" @click="openBrowser(whatsappLink)">5440 7482</a>
              </div>
            </div>
            <div class="mobile-nav">
              <ul
                :style="`display: ${mobileToggle ? 'block' : 'none'}`"
                class="open"
              >
                <li class="active has-sub-item">
                  <span class="submenu-button submenu-opened"></span
                  ><a href="#Banner">主頁</a>
                </li>
                <li><nuxt-link to="#About">關於我們</nuxt-link></li>
                <li class="has-sub-item">
                  <span class="submenu-button"></span>
                  <a href="#Blog">Blog</a>
                </li>
                <li><nuxt-link to="#Contact">聯絡我們</nuxt-link></li>
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
  name: 'NavTwo',
  data() {
    return {
      sticky: false,
      mobileToggle: false,
      whatsappLink:
        'https://api.whatsapp.com/send?phone=85254407482&app=facebook&entry_point=page_cta&fbclid=IwAR155hKk6PZq-9X0jaivk57VMwjiRSJCj02Ej2IhHozW_Pkr2X9oVf56gM8'
    };
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
        this.sticky = true;
      } else if (window.scrollY < 70) {
        this.sticky = false;
      }
    }
  }
};
</script>

<style scoped>
.main-header.header-style2 {
  background-color: #4eddad;
}

.main-logo {
  width: 80px;
}

a {
  font-family: 'genJyuuGothic-regular';
  font-size: 20px;
  line-height: 1.5;
}
</style>
