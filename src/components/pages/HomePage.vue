<template>
  <div class="home-hero">
    <section id="hero" class="hero section">
      <ul class="social-icon">
        <li class="icon-list icon-list-vk">
          <a href="https://vk.com/malyaevbmx" target="_blank" class="icon-text">
            <i class="bi bi-vimeo"></i>
          </a>
        </li>
        <li class="icon-list icon-list-youtube">
          <a href="#" target="_blank" class="icon-text">
            <i class="bi bi-youtube"></i>
          </a>
        </li>
      </ul>
      <img v-once src="../../assets/images/main.jpg" alt="" data-aos="fade-in" />
      <div
        class="container text-center"
        data-aos="fade-up"
        data-aos-delay="100"
      >
        <div class="row justify-content-center">
          <div class="col-lg-8">
            <p>Превращаем катание в искусство</p>
            <h2>Велошкола<br />&#761;CENTR&#764;</h2>
            <a
              href="https://vk.com/im?sel=-225474558"
              target="_blank"
              class="btn-get-started"
              >Записаться</a
            >
          </div>
        </div>
        <div class="product box-shadow d-md-block"></div>
        <div class="product-2 box-shadow d-md-block"></div>
      </div>
    </section>
  </div>
</template>

<style type="text/scss">
section,
.section {
  color: var(--default-color);
  background-color: var(--background-color);
  padding: 60px 0;
  scroll-margin-top: 90px;
  overflow: clip;
}

.home-hero {
  .product {
    position: absolute;
    right: 0;
    left: auto;
    bottom: 0;
    width: 230px;
    height: 230px;
    box-shadow: 10px 10px 0 0 var(--accent-color);
  }

  .product-2 {
    position: absolute;
    top: 0;
    right: auto;
    bottom: 0;
    left: 0;
    width: 230px;
    height: 230px;
    box-shadow: 10px 10px 0 0 var(--accent-color);
    transform: rotate(180deg);
  }

  .social-icon {
    z-index: 4;
    position: absolute;
    top: 60%;
    left: 3%;
    margin: 0;
    padding: 0;
    list-style: none;

    .icon-list {
      margin-right: 2rem;
      width: 30px;
      height: 30px;
      background: rgba(0, 0, 0, 0.65);
      border-radius: 50%;
      text-align: center;
      margin-bottom: 10px;
      -webkit-transition: all 0.3s;
      -o-transition: all 0.3s;
      transition: all 0.3s;
    }

    .icon-list:hover {
      background: var(--accent-color);
    }

    .icon-list-vk:hover {
      background: var(--vk-color);
    }

    .icon-list-youtube:hover {
      background: var(--youtube-color);
    }

    .icon-text {
      font-size: 12px;
      line-height: 30px;
      -webkit-transition: all 0.3s ease;
      -o-transition: all 0.3s ease;
      transition: all 0.3s ease;
      color: #fff;
    }
  }

  .hero {
    width: 100%;
    min-height: 100vh;
    position: relative;
    padding: 80px 0;
    display: flex;
    align-items: center;
    justify-content: center;

    img {
      position: absolute;
      inset: 0;
      display: block;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: 1;
    }

    .container {
      position: relative;
      z-index: 3;
      padding: 10px;
      background-color: rgba(0, 0, 0, 0.5);
      border-radius: 20px;
    }

    h2 {
      margin: 0;
      text-align: left;
      font-size: 110px;
      font-weight: 800;
    }

    @media (max-width: 768px) {
      h2 {
        font-size: 60px;
      }
    }
  }

  .hero:before {
    content: "";
    position: absolute;
    inset: 0;
    z-index: 2;
  }

  p {
    text-align: left;
    margin: 10px 0 0 0;
    font-size: 24px;
    color: var(--default-color);
  }

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
    background: inherit;
    border-color: var(--accent-color);
  }

  @media (max-width: 768px) {
    h2 {
      font-size: 32px;
    }

    p {
      font-size: 18px;
    }

    .hero {
      min-height: 0;
    }
  }
}
</style>
