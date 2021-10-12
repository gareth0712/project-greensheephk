<template>
  <section id="Contact" class="pt-120 pb-100">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-md-8">
          <!-- cta title -->
          <div class="callto-heading">
            <span class="schoolbell">做好風險管理 讓財富穩健增長</span>
            <h2 class="text-blue">立即登記<br />領取你的專屬累積財富方案</h2>
          </div>
          <!-- cta title -->
        </div>
        <div class="col-md-4">
          <div class="call-action-btn text-right">
            <div @click="openBrowser(whatsappLink)" class="btn">立即登記</div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'CallToAction',
  data() {
    return {
      whatsappLink:
        'https://api.whatsapp.com/send?phone=85254407482&app=facebook&entry_point=page_cta&fbclid=IwAR0EM0JoH7Iqs4fJk-Dz3NDpr1fyAUECCNICPy7xz3js9tLFeL8t-whWFPY'
    };
  },
  methods: {
    openBrowser(link) {
      if (!link) return;
      window.open(link);
    }
  }
};
</script>

<style scoped>
#Contact {
  background-color: #f0f3bd;
}

.schoolbell {
  font-family: 'genJyuuGothic-medium';
}

.text-blue {
  font-family: 'genJyuuGothic-medium';
}

.btn {
  font-family: 'genJyuuGothic-regular';
}
</style>
