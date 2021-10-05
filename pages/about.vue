<template>
  <div>
    <NavOne />
    <PageHeader title="About Us" />
    <Features />
    <AboutArea />
    <Team />
    <TestimonialTwo />
    <ClientsLogoTwo />
    <Footer />
  </div>
</template>
<script>
  import NavOne from "../components/NavOne";
  import Footer from "../components/Footer";
  import PageHeader from "../components/PageHeader";
  import Features from "../components/Features";
  import AboutArea from "../components/AboutArea";
  import Team from "../components/Team";
  import TestimonialTwo from "../components/TestimonialTwo";
  import ClientsLogoTwo from "../components/ClientsLogoTwo";
  export default {
    components: {
      ClientsLogoTwo,
      TestimonialTwo,
      Team,
      AboutArea,
      Features,
      PageHeader,
      Footer,
      NavOne
    },
    head(){
      return {
        title: "Mineralo - About Us"
      }
    },

  }
</script>
