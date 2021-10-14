<template>
  <div>
    <Nav />
    <Banner />
    <CallToAction />
    <About />
    <Blog />
    <Footer />
  </div>
</template>
<script>
import Nav from '../components/Nav';
import Banner from '../components/Banner';
import Footer from '../components/Footer';
import About from '../components/About';
import Blog from '../components/Blog';
import CallToAction from '../components/CallToAction';
export default {
  components: {
    Nav,
    Banner,
    About,
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
