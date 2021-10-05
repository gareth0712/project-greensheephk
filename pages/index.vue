<template>
  <div>
    <NavOne />
    <BannerOne />
    <FeatureArea />
    <Video />
    <BottleDeliver />
    <FeatureAreaTwo />
    <AboutArea />
    <Team />
    <Subscribe />
    <Testimonial />
    <Location />
    <ClientsLogo />
    <Footer />
  </div>
</template>

<script>
  import NavOne from "../components/NavOne";
  import BannerOne from "../components/BannerOne";
  import Footer from "../components/Footer";
  import FeatureArea from "../components/FeatureArea";
  import Video from "../components/Video";
  import BottleDeliver from "../components/BottleDeliver";
  import FeatureAreaTwo from "../components/FeatureAreaTwo";
  import AboutArea from "../components/AboutArea";
  import Team from "../components/Team";
  import Subscribe from "../components/Subscribe";
  import Testimonial from "../components/Testimonial";
  import Location from "../components/Location";
  import ClientsLogo from "../components/ClientsLogo";
  export default {
    components: {
      ClientsLogo,
      Location,
      Testimonial,
      Subscribe,
      Team,
      AboutArea,
      FeatureAreaTwo,
      BottleDeliver,
      Video,
      FeatureArea,
      Footer,
      BannerOne,
      NavOne
    }
  }
</script>
