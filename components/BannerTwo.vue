<template>
  <div id="Banner" class="banner-area-inner">
    <div class="banner-wrap home-banner2" />
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
  background-size: cover;
}
</style>
