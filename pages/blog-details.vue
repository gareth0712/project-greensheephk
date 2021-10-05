<template>
  <div>
    <NavOne />
    <PageHeader title="Blog Detail" />
    <BlogDetails />
    <Footer />
  </div>
</template>
<script>
  import NavOne from "../components/NavOne";
  import PageHeader from "../components/PageHeader";
  import BlogPage from "../components/BlogPage";
  import Footer from "../components/Footer";
  import BlogDetails from "../components/BlogDetails";
  export default {
    components: {
      BlogDetails,
      Footer,
      BlogPage,
      PageHeader,
      NavOne
    },
    head(){
      return {
        title: "Mineralo - Blog Detail"
      }
    },
  }
</script>
