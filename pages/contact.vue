<template>
  <div>
    <NavOne />
    <PageHeader title="Contact" />
    <Contact />
    <MapG />
    <Footer />
  </div>
</template>
<script>
  import NavOne from "../components/NavOne";
  import PageHeader from "../components/PageHeader";
  import Contact from "../components/Contact";
  import MapG from "../components/MapG";
  import Footer from "../components/Footer";
  export default {
    components: {
      Footer,
      MapG,
      Contact,
      PageHeader,
      NavOne
    },
    head(){
      return {
        title: "Mineralo - Contact"
      }
    },
  }
</script>
