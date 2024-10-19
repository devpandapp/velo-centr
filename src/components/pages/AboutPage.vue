<template>
  <div class="home-about" id="about">
    <div class="floating-icon" id="service_info_item">
      <div class="floating-icon__is floating-icon-info">
        <i class="flaticon-phone"></i>
      </div>
      <div class="floating-icon__is floating-icon-location">
        <i class="flaticon-pin"></i>
      </div>
      <div class="floating-icon__is floating-icon-message">
        <i class="flaticon-mail"></i>
      </div>
    </div>
    <div class="container">
      <div class="row">
        <div class="about-title">О нас</div>
      </div>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-lg-6">
          <div class="row">
            <div class="about-image">
              <img v-once src="../../assets/images/about.jpg" alt="About" />
              <div class="overlay-content">
                Профессиональные тренеры, индивидуальный подход к каждому
                ученику и современные методики обучения. Мы поможем вам освоить
                новый вид спорта или улучшить свои навыки.
              </div>
              <span class="about-line"></span>
            </div>
          </div>
        </div>
        <div class="col-lg-6 park-section">
          <h1 class="park-title">Наш парк</h1>
          <div class="row">
            <div class="col-lg-4 col-md-12 mb-4 mb-lg-0">
              <img
                v-once
                src="../../assets/images/park1.jpg"
                class="w-100 shadow-1-strong rounded mb-4"
                alt="Park1"
              />
              <img
                v-once
                src="../../assets/images/park2.jpg"
                class="w-100 shadow-1-strong rounded mb-4"
                alt="Park2"
              />
            </div>
            <div class="col-lg-4 mb-4 mb-lg-0">
              <img
                v-once
                src="../../assets/images/park3.jpg"
                class="w-100 shadow-1-strong rounded mb-4"
                alt="Park3"
              />
              <img
                v-once
                src="../../assets/images/park4.jpg"
                class="w-100 shadow-1-strong rounded mb-4"
                alt="Park4"
              />
            </div>
            <div class="col-lg-4 mb-4 mb-lg-0">
              <img
                v-once
                src="../../assets/images/park5.jpg"
                class="w-100 shadow-1-strong rounded mb-4"
                alt="Park5"
              />
              <img
                v-once
                src="../../assets/images/park6.jpg"
                class="w-100 shadow-1-strong rounded mb-4"
                alt="Park6"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style type="text/scss">
.home-about {
  .about-title {
    margin-top: 75px;
    font-weight: 900;
    margin-bottom: 45px;
    font-size: 110px;
  }

  @media (max-width: 768px) {
    .about-title {
      font-size: 60px;
    }
  }

  .about-image {
    padding: 0;
    position: relative;

    img {
      max-width: 100%;
    }

    .overlay-content {
      width: 80%;
      color: white;
      left: 47% !important;
      position: absolute;
      background: rgba(0, 0, 0, 0.7);
      top: 50%;
      -webkit-transform: translate(-50%, -50%);
      -ms-transform: translate(-50%, -50%);
      transform: translate(-50%, -50%);
      font-size: 18px;
      letter-spacing: 0.45px;
      line-height: 35px;
      padding: 30px 30px;
    }

    .about-line {
      position: absolute;
      width: 10px;
      height: 100px;
      background: var(--accent-color);
      top: -62px;
      left: 91px;
    }
  }

  .park-section {
    margin-top: 26px;
    align-content: center;

    .park-title {
      border-bottom: 4px solid var(--accent-color);
    }
  }
}
</style>
