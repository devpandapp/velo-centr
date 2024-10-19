<template>
  <div class="home-services" id="services">
    <div class="container">
      <div class="col-lg-12 text-center">
        <div class="top-text">
          <div>
            Секции
            <span class="services-line"></span>
          </div>
        </div>
      </div>
      <div class="row row-cols-1 row-cols-md-3 g-4">
        <div class="col">
          <div class="card h-100">
            <img v-once
              src="../../assets/images/begovel.jpg"
              class="card-img-top"
              alt="..."
            />
            <div class="card-body">
              <h2 class="card-title">Беговел</h2>
              <h5 class="card-text">Для детей от 3 лет</h5>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="card h-100">
            <div class="card-body">
              <h2 class="card-title">Скейтборд</h2>
              <h5 class="card-text">Для уверенных райдеров</h5>
            </div>
            <img v-once
              src="../../assets/images/skeit.png"
              class="card-img-bottom"
              alt="..."
            />
          </div>
        </div>
        <div class="col">
          <div class="card h-100">
            <img v-once
              src="../../assets/images/bmx.png"
              class="card-img-top"
              alt="..."
            />
            <div class="card-body">
              <h2 class="card-title">BMX</h2>
              <h5 class="card-text">Для любителей экстрима</h5>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="card h-100">
            <div class="card-body">
              <h2 class="card-title">Велосипед</h2>
              <h5 class="card-text">Обучение езде с нуля</h5>
            </div>
            <img v-once
              src="../../assets/images/velosiped.jpg"
              class="card-img-bottom"
              alt="..."
            />
          </div>
        </div>
        <div class="col">
          <div class="card h-100">
            <img v-once
              src="../../assets/images/roliki.png"
              class="card-img-top"
              alt="..."
            />
            <div class="card-body">
              <h2 class="card-title">Ролики</h2>
              <h5 class="card-text">Для любителей скорости и манёвренности</h5>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="card h-100">
            <div class="card-body">
              <h2 class="card-title">Самокат</h2>
              <h5 class="card-text">
                Для тех, кто хочет быть мобильным и активным
              </h5>
            </div>
            <img v-once
              src="../../assets/images/samokat.png"
              class="card-img-bottom"
              alt="..."
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style type="text/scss">
.home-services {
  margin-top: 58px;

  .top-text {
    font-size: 110px;
    margin-bottom: 45px;
    font-weight: 900;
  }

  @media (max-width: 768px) {
    .top-text {
      font-size: 60px;
    }
  }

  .services-line {
    position: absolute;
    width: 120px;
    height: 10px;
    background: var(--accent-color);
    right: 0px;
  }

  .card-body {
    .card-text {
      font-weight: normal;
    }
  }
}
</style>
