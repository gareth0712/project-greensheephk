<template>
  <div class="page-title-wrap primary-bg">
      <div class="container">
          <div class="row">
              <div class="col">
                  <!-- page title content -->
                  <div class="page-title-content text-center">
                      <ul class="mb-0 list-unstyle nav">
                          <li><nuxt-link to="/">Home</nuxt-link></li>
                          <li><a href="#">{{ title }}</a></li>
                      </ul>
                      <h1 class="h2">{{ title }}</h1>
                  </div><!-- /.End of page title content -->
              </div><!-- /.col -->
          </div><!-- /.row -->
      </div><!-- /.container -->
  </div>
</template>

<script>
    export default {
      name: "PageHeader",
      props: {
        title: {
          type: String
        }
      }
    }
</script>

<style scoped>

</style>
