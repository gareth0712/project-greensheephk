<template>
  <section id="About" class="pt-120 pb-120 quality">
    <div class="container">
      <div class="row">
        <div class="about-logo">
          <img src="/about.png" />
        </div>
        <div class="col-md-6 about-text">
          <!-- section title -->
          <div class="title">關於懶羊羊理財</div>
          <!-- End of section title -->
          <div class="our-quality-inner">
            <p>
              一家四口中產家庭將「懶洋洋達到財務自由」為終極目標，將有限資金作有效配置，秒秒鐘躺著收錢！懶羊羊爸爸汲取投資失利的教訓，做好風險管理，穩健累積財富！
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'QualityArea'
};
</script>

<style scoped>
#About {
  min-height: 900px;
  padding-bottom: 0px;
  padding-top: 0px;
  background-color: #b5e61d;
}

.title {
  margin-bottom: 88px;
  font-size: 50px;
  color: #0e0e0e;
  font-family: 'genJyuuGothic-bold';
}

h2::after {
  content: '';
  width: 0px;
  height: 0px;
}

.container {
  max-width: 100%;
  min-height: 900px;
}

.row {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  max-height: 100%;
  min-height: 900px;
  padding: 30px;
}

.about-logo {
  width: 50%;
  margin-right: 80px;
  max-width: 600px;
}

.about-text {
  width: 40%;
  max-width: 400px;
}

@media (max-width: 991.98px) {
  #About {
    min-height: 850px;
    padding-bottom: 0px;
    padding-top: 0px;
    background-color: #b5e61d;
  }

  .title {
    margin-bottom: 48px;
  }

  .container {
    max-width: 100%;
    min-height: 900px;
  }

  .row {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100%;
    max-height: 100%;
    min-height: 900px;
    padding: 30px;
  }

  .about-logo {
    width: fit-content;
    margin: 0px;
    max-width: 600px;
  }

  .about-text {
    margin-top: 60px;
    width: fit-content;
  }
}

@media screen and (max-width: 480px) {
  #About {
    min-height: 700px;
  }
  .title {
    font-size: 40px;
    text-align: center;
  }

  .row {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
  }

  .container {
    max-width: 100%;
    min-height: 700px;
  }

  .about-text {
    margin-top: 40px;
    width: fit-content;
  }
}
</style>
