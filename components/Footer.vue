<template>
  <div>
    <!-- footer -->
    <footer class="footer">
      <div class="footer-top pt-110 pb-70">
        <div class="container">
          <div class="row">
            <div class="col-md-4">
              <!-- footer widget -->
              <div class="footer-widget text-center">
                <div class="widget-title">
                  <h3>Follow</h3>
                </div>
                <div class="footer-social-area">
                  <ul class="social-list mb--0 list-unstyled">
                    <li>
                      <a
                        class="follow-button"
                        @click="openBrowser(instagramLink)"
                      >
                        <i class="fa fa-instagram" />
                      </a>
                    </li>
                    <li>
                      <a
                        class="follow-button"
                        @click="openBrowser(facebookLink)"
                      >
                        <i class="fa fa-facebook" />
                      </a>
                    </li>
                    <!-- <li>
                      <a
                        class="follow-button"
                        @click="openBrowser(youtubeLink)"
                      >
                        <i class="fa fa-youtube" />
                      </a>
                    </li> -->
                  </ul>
                </div>
              </div>
              <!-- End of footer widget -->
            </div>

            <div class="col-md-4">
              <!-- footer widget -->
              <div class="footer-widget text-right">
                <div class="widget-title">
                  <h3>Contact</h3>
                </div>
                <div class="footer-contact-info">
                  <div class="whatsapp" @click="openBrowser(whatsappLink)">
                    <i class="fa fa-whatsapp" />
                    5440 7482
                  </div>
                  <a class="email" :href="`mailto:${email}`"
                    ><i class="fa fa-envelope" />{{ email }}</a
                  >
                </div>
              </div>
              <!-- End of footer widget -->
            </div>
          </div>
        </div>
      </div>
      <div class="footer-bottom text-center" />
    </footer>
    <!-- End of footer -->

    <!-- back to top -->
    <div @click="scrollTop" :class="`back-to-top ${scrollBtn ? 'show' : ''}`">
      <a href="#"><i class="fa fa-chevron-up"/></a>
    </div>
    <!-- back to top -->
  </div>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      scrollBtn: false,
      email: 'moneysheephk@gmail.com',
      whatsappLink:
        'https://api.whatsapp.com/send?phone=85254407482&app=facebook&entry_point=page_cta&fbclid=IwAR155hKk6PZq-9X0jaivk57VMwjiRSJCj02Ej2IhHozW_Pkr2X9oVf56gM8',
      facebookLink: 'https://www.facebook.com/moneysheephk',
      instagramLink: 'https://instagram.com/moneysheephk',
      youtubeLink: ''
    };
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      if (window.scrollY > 70) {
        this.scrollBtn = true;
      } else if (window.scrollY < 70) {
        this.scrollBtn = false;
      }
    },
    openBrowser(link) {
      if (!link) return;
      window.open(link);
    },

    scrollTop() {
      window.scrollTo(0, 0);
    }
  }
};
</script>

<style scoped>
.footer-widget {
  min-width: 260px;
}

.row {
  justify-content: center;
}

.fa-whatsapp,
.fa-envelope {
  margin-right: 8px;
}

.footer {
  background-color: #02806f;
}

.follow-button {
  background-color: #05668d;
}

.follow-button,
.whatsapp,
.email {
  cursor: pointer;
  color: #f0f0f0 !important;
}
</style>
