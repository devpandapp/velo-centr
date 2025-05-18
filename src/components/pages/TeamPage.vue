<template>
  <div class="home-team" id="team">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="content">
            <h1 class="home-team-title">Наша команда</h1>
            <span id="line"></span>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-6">
          <div class="row">
            <div class="col-lg-6 image-text-center">
              <img v-once src="../../assets/images/person.jpg" />
            </div>
            <div class="col-lg-6">
              <div class="content-bottom">
                <h1 class="title">Дмитрий Маляев</h1>
                <span class="text"
                  >Директор и тренер велошколы "CENTR". Профессиональный BMX
                  райдер.</span
                >
              </div>
            </div>
          </div>
        </div>
        <!-- <div class="col-lg-6">
          <div class="row">
            <div class="col-lg-6 image-text-center">
              <img v-once src="../../assets/images/person.png" />
            </div>
            <div class="col-lg-6">
              <div class="content-bottom">
                <h1 class="title">Человек 2</h1>
                <span class="text"
                  >Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                  Nulla sit amet semper augue. Maecenas gravida tortor sit amet
                  enim venenatis tristique. Nulla vehicula porta tortor non
                  maximus.</span
                >
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-6">
          <div class="row">
            <div class="col-lg-6">
              <div class="content-bottom">
                <h1 class="title">Человек 3</h1>
                <span class="text"
                  >Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                  Nulla sit amet semper augue. Maecenas gravida tortor sit amet
                  enim venenatis tristique. Nulla vehicula porta tortor non
                  maximus.</span
                >
              </div>
            </div>
            <div class="col-lg-6 image-text-center">
              <img v-once src="../../assets/images/person.png" />
            </div>
          </div>
        </div>
        <div class="col-lg-6">
          <div class="row">
            <div class="col-lg-6">
              <div class="content-bottom">
                <h1 class="title">Человек 4</h1>
                <span class="text"
                  >Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                  Nulla sit amet semper augue. Maecenas gravida tortor sit amet
                  enim venenatis tristique. Nulla vehicula porta tortor non
                  maximus.</span
                >
              </div>
            </div>
            <div class="col-lg-6 image-text-center">
              <img v-once src="../../assets/images/person.png" />
            </div>
          </div>
        </div> -->
      </div>
    </div>
  </div>
</template>

<style type="text/scss">
.home-team {
  margin-top: 74px;

  .content {
    margin-bottom: 75px;
    text-align: center;

    .home-team-title {
      font-family: var(--body-font);
      font-size: 110px;
      font-weight: 900;
      text-align: center;
      letter-spacing: 0.025em;
      color: var(--heading-color);
      line-height: 150px;
    }

    @media (max-width: 768px) {
      .home-team-title {
        font-size: 60px;
        line-height: 55px;
      }
    }

    span {
      font-family: var(--body-font);
      font-size: 22px;
      font-weight: 500;
      letter-spacing: 0.025em;
      color: var(--heading-color);
    }
  }

  .content-bottom {
    margin-top: 40px;
    margin-bottom: 40px;

    .title {
      font-size: 30px;
      font-family: var(--body-font);
      font-weight: 600;
      color: var(--heading-color);
      text-align: left;
      margin-bottom: 40px;
      position: relative;
    }

    .title:before {
      content: "";
      height: 3px;
      background: var(--main-color);
      width: 100%;
      bottom: -40%;
      position: absolute;
    }

    .text {
      font-size: 18px;
      font-family: var(--body-font);
      font-weight: 400;
      color: var(--heading-color);
      text-align: left;
      letter-spacing: 0.025em;
    }
  }

  .image-text-center {
    text-align: center;
  }

  img {
    -webkit-box-shadow: 0px 0px 6px #ccc;
    box-shadow: 0px 0px 6px #ccc;
  }

  #line {
    position: absolute;
    width: 10px;
    height: 100px;
    background: var(--accent-color);
  }
}
</style>
