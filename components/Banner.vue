<template>
  <div id="Banner" class="banner-area-inner">
    <div class="banner-wrap home-banner2" />
    <img src="/banner_mobile.png" class="alternate-banner" v-if="isMobile" />
  </div>
</template>

<script>
export default {
  name: 'BannerTwo',
  data() {
    return {
      isMobile: false
    };
  },
  methods: {
    handleResize() {
      if (window.outerWidth <= 991) {
        if (!this.isMobile) this.isMobile = true;
        return;
      }
      if (this.isMobile) this.isMobile = false;
    }
  },
  mounted() {
    this.handleResize();
    window.addEventListener('resize', this.handleResize);
  },
  destroyed() {
    window.removeEventListener('resize', this.handleResize);
  }
};
</script>

<style scoped>
.banner-area-inner {
  padding-top: 100px;
  padding-bottom: 0px;
  background-color: #4eddad;
  min-height: 700px;
  height: 80vh;
}

.banner-wrap.home-banner2 {
  background-image: url('/banner.png');
}

.alternatve-banner {
  width: 100%;
}

@media (max-width: 991.98px) {
  .banner-area-inner {
    min-height: 100px;
    max-height: 634px;
    height: fit-content;
    padding-bottom: 40px;
  }

  .banner-wrap.home-banner2 {
    display: none;
    background-image: unset;
  }

  .alternatve-banner {
    display: block;
  }
}
</style>
