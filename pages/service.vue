<template>
  <div>
    <NavOne />
    <PageHeader title="Service" />
    <Service />
    <FeatureAreaTwo />
    <FeaturesTwo />
    <ClientsLogo />
    <Footer />
  </div>
</template>
<script>
  import NavOne from "../components/NavOne";
  import Footer from "../components/Footer";
  import PageHeader from "../components/PageHeader";
  import FeaturesTwo from "../components/FeaturesTwo";
  import Service from "../components/Service";
  import ClientsLogo from "../components/ClientsLogo";
  import FeatureAreaTwo from "../components/FeatureAreaTwo";
  export default {
    components: {
      FeatureAreaTwo,
      ClientsLogo,
      FeaturesTwo,
      PageHeader,
      Footer,
      NavOne,
      Service
    },
    head(){
      return {
        title: "Mineralo - Service"
      }
    },

  }
</script>
