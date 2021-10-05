<template>
  <div>
    <NavTwo />
    <BannerThree />
    <FeatureAreaFour />
    <QualityArea />
    <BottleDeliver />
    <Testimonial />
    <LocationTwo />
    <Blog />
    <CallToAction />
    <Footer />
  </div>
</template>
<script>
  import NavTwo from "../components/NavTwo";
  import Footer from "../components/Footer";
  import BannerThree from "../components/BannerThree";
  import FeatureAreaFour from "../components/FeatureAreaFour";
  import QualityArea from "../components/QualityArea";
  import BottleDeliver from "../components/BottleDeliver";
  import Testimonial from "../components/Testimonial";
  import LocationTwo from "../components/LocationTwo";
  import Blog from "../components/Blog";
  import CallToAction from "../components/CallToAction";
  export default {
    components: {
      Footer,
      NavTwo,
      BannerThree,
      FeatureAreaFour,
      QualityArea,
      BottleDeliver,
      Testimonial,
      LocationTwo,
      Blog,
      CallToAction,
    },
    head(){
      return {
        title: "Mineralo - Home 3"
      }
    },
  }
</script>
