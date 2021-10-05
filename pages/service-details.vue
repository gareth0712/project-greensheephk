<template>
  <div>
    <NavOne />
    <PageHeader title="Service Detail" />
    <ServiceDetails />
    <Location />
    <ClientsLogo />
    <Footer />
  </div>
</template>
<script>
  import NavOne from "../components/NavOne";
  import PageHeader from "../components/PageHeader";
  import Footer from "../components/Footer";
  import ServiceDetails from "../components/ServiceDetails";
  import Location from "../components/Location";
  import ClientsLogo from "../components/ClientsLogo";
  export default {
    components: {
      ClientsLogo,
      Location,
      Footer,
      PageHeader,
      NavOne,
      ServiceDetails
    },
    head(){
      return {
        title: "Mineralo - Service Detail"
      }
    },

  }
</script>
