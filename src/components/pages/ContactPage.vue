<template>
  <div class="home-contact" id="contact">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <div>
            <h1 class="contact-title">Связаться с нами</h1>
          </div>
        </div>
      </div>
      <div class="row contact-row">
        <div class="col-lg-6">
          <iframe
            class="ya-map"
            src="https://yandex.com/map-widget/v1/?ll=49.377711%2C53.544543&mode=search&oid=128953636295&ol=biz&z=18"
            width="100%"
            height="400"
            frameborder="1"
            allowfullscreen="true"
          ></iframe>
        </div>
        <div class="col-lg-6">
          <div class="contact-right">
            <div class="card-body p-md-4">
              <h4 class="text-uppercase mb-4">Велошкола "CENTR"</h4>
              <div class="row mb-1">
                <div class="col-md-12">
                  <div
                    data-mdb-input-init=""
                    class="form-outline"
                    data-mdb-input-initialized="true"
                  >
                    <label class="form-label"
                      >445004, Россия, Самарская область, Тольятти, Южное шоссе,
                      5, 2-й этаж</label
                    >
                  </div>
                </div>
              </div>
              <div class="row mb-3">
                <div class="col-md-12">
                  <div
                    data-mdb-input-init=""
                    class="form-outline"
                    data-mdb-input-initialized="true"
                  >
                    <a
                      href="tel: 89370609029"
                      class="btn btn-outline-danger"
                      role="button"
                    >
                      <i class="bi bi-telephone-fill"></i> +7 (937) 060-90-29
                    </a>
                  </div>
                </div>
              </div>
              <div class="btn-group" role="group">
                <a
                  href="https://vk.com/malyaevbmx"
                  class="btn btn-outline-primary"
                  role="button"
                  target="_blank"
                >
                  <i class="bi bi-vimeo"></i> Вконтакте
                </a>
                <a
                  href="https://wa.me/79370609029"
                  class="btn btn-outline-success"
                  role="button"
                  target="_blank"
                >
                  <i class="bi bi-whatsapp"></i> Whatsapp
                </a>
                <a
                  href="http://t.me/malyaevbmx"
                  class="btn btn-outline-info"
                  role="button"
                  target="_blank"
                >
                  <i class="bi bi-telegram"></i> Telegram
                </a>
              </div>
            </div>
          </div>
          <div class="contact-right-button">
            <div class="card-body p-md-5 mt-5">
              <div class="row">
                <div class="col-md-12">
                  <div
                    data-mdb-input-init=""
                    class="form-outline"
                    data-mdb-input-initialized="true"
                  >
                    <a
                      href="https://vk.com/im?sel=-225474558"
                      target="_blank"
                      class="btn-get-started"
                      >Записаться</a
                    >
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style type="text/scss">
.home-contact {
  margin-top: 84px;

  .contact-title {
    font-family: var(--body-font);
    font-size: 110px;
    font-weight: 900;
    text-align: center;
    letter-spacing: 0.025em;
    color: var(--heading-color);
    border-bottom: 10px solid var(--accent-color);
    margin-bottom: 58px;
    line-height: 150px;
  }

  @media (max-width: 768px) {
    .contact-title {
      font-size: 55px;
      line-height: 55px;
      padding-bottom: 30px;
    }
  }

  .contact-row {
    .ya-map {
      position: relative;
    }

    .form-label {
      margin-left: 0px;
    }
  }

  .contact-right-button {
    text-align: center;

    .btn-get-started {
      color: var(--default-color);
      font-weight: 400;
      font-size: 16px;
      letter-spacing: 1px;
      display: inline-block;
      padding: 8px 40px;
      margin: 30px 0 0 0;
      border-radius: 50px;
      transition: 0.5s;
      border: 2px solid var(--accent-color);
      background: var(--accent-color);
      text-decoration: none;
    }

    .btn-get-started:hover {
      color: var(--accent-color);
      background: inherit;
      border-color: var(--accent-color);
    }
  }
}
</style>
