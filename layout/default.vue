<template>
  <nuxt />
</template>

<script>
export default {
  components: {},
  head() {
    return {
      title: 'MoneySheephk 懶羊羊理財'
    };
  },
  mounted() {
    this.$nextTick(() => {
      this.$nuxt.$loading.start();
      setTimeout(() => this.$nuxt.$loading.finish(), 500);
    });
  }
};
</script>

<style></style>
