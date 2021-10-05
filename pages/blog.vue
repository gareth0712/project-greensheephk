<template>
  <div>
    <NavOne />
    <PageHeader title="Blog" />
    <BlogPage />
    <Footer />
  </div>
</template>
<script>
  import NavOne from "../components/NavOne";
  import PageHeader from "../components/PageHeader";
  import BlogPage from "../components/BlogPage";
  import Footer from "../components/Footer";
  export default {
    components: {Footer, BlogPage, PageHeader, NavOne},
    head(){
      return {
        title: "Mineralo - Blog"
      }
    },
  }
</script>
