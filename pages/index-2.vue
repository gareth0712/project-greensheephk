<template>
  <div>
    <NavTwo />
    <BannerTwo />
    <LifeSaferArea />
    <FeatureAreaThree />
    <FeatureAreaTwo />
    <QualityArea />
    <BottleDeliver />
    <TestimonialTwo />
    <Blog />
    <MapG />
    <CallToAction />
    <Footer />
  </div>
</template>
<script>
  import NavTwo from "../components/NavTwo";
  import BannerTwo from "../components/BannerTwo";
  import Footer from "../components/Footer";
  import LifeSaferArea from "../components/LifeSaferArea";
  import FeatureAreaThree from "../components/FeatureAreaThree";
  import FeatureAreaTwo from "../components/FeatureAreaTwo";
  import QualityArea from "../components/QualityArea";
  import BottleDeliver from "../components/BottleDeliver";
  import TestimonialTwo from "../components/TestimonialTwo";
  import Blog from "../components/Blog";
  import MapG from "../components/MapG";
  import CallToAction from "../components/CallToAction";
  export default {
    components: {
      CallToAction,
      MapG,
      Blog,
      TestimonialTwo,
      BottleDeliver,
      QualityArea,
      FeatureAreaTwo,
      FeatureAreaThree,
      LifeSaferArea,
      Footer,
      BannerTwo,
      NavTwo
    },
    head(){
      return {
        title: "Mineralo - Home 2"
      }
    },
  }
</script>
