<template>
  <div>
    <NavTwo />
    <BannerTwo />
    <QualityArea />
    <BottleDeliver />
    <TestimonialTwo />
    <Blog />
    <CallToAction />
    <Footer />
  </div>
</template>
<script>
import NavTwo from '../components/NavTwo';
import BannerTwo from '../components/BannerTwo';
import Footer from '../components/Footer';
import QualityArea from '../components/QualityArea';
import BottleDeliver from '../components/BottleDeliver';
import TestimonialTwo from '../components/TestimonialTwo';
import Blog from '../components/Blog';
import CallToAction from '../components/CallToAction';
export default {
  components: {
    NavTwo,
    BannerTwo,
    QualityArea,
    TestimonialTwo,
    BottleDeliver,
    Blog,
    CallToAction,
    Footer
  },
  head() {
    return {
      title: 'Money Sheep 懶羊羊理財'
    };
  }
};
</script>
