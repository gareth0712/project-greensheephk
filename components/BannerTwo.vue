<template>
  <div id="Banner" class="banner-area-inner">
    <div class="banner-wrap home-banner2" />
    <img src="/banner_mobile.png" class="alternate-banner" />
  </div>
</template>

<script>
export default {
  name: 'BannerTwo'
};
</script>

<style scoped>
.banner-area-inner {
  padding-top: 100px;
  padding-bottom: 100px;
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
