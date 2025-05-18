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
                  href="https://vk.com/centrschool63"
                  class="btn btn-outline-primary"
                  role="button"
                  target="_blank"
                >
                  <svg
                    width="19"
                    height="18"
                    viewBox="0 0 101 100"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <g clip-path="url(#clip0_2_40)">
                      <path
                        d="M0.5 48C0.5 25.3726 0.5 14.0589 7.52944 7.02944C14.5589 0 25.8726 0 48.5 0H52.5C75.1274 0 86.4411 0 93.4706 7.02944C100.5 14.0589 100.5 25.3726 100.5 48V52C100.5 74.6274 100.5 85.9411 93.4706 92.9706C86.4411 100 75.1274 100 52.5 100H48.5C25.8726 100 14.5589 100 7.52944 92.9706C0.5 85.9411 0.5 74.6274 0.5 52V48Z"
                        fill="#0077FF"
                      />
                      <path
                        d="M53.7085 72.042C30.9168 72.042 17.9169 56.417 17.3752 30.417H28.7919C29.1669 49.5003 37.5834 57.5836 44.25 59.2503V30.417H55.0004V46.8752C61.5837 46.1669 68.4995 38.667 70.8329 30.417H81.5832C79.7915 40.5837 72.2915 48.0836 66.9582 51.1669C72.2915 53.6669 80.8336 60.2086 84.0836 72.042H72.2499C69.7082 64.1253 63.3754 58.0003 55.0004 57.1669V72.042H53.7085Z"
                        fill="white"
                      />
                    </g>
                    <defs>
                      <clipPath id="clip0_2_40">
                        <rect
                          width="100"
                          height="100"
                          fill="white"
                          transform="translate(0.5)"
                        />
                      </clipPath>
                    </defs>
                  </svg>
                  Вконтакте
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
