<template>
  <div class="home-hero">
    <section id="hero" class="hero section">
      <ul class="social-icon">
        <li class="icon-list icon-list-vk">
          <a
            href="https://vk.com/centrschool63"
            target="_blank"
            class="icon-text"
          >
            <svg
              width="21"
              height="20"
              viewBox="0 0 101 100"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g clip-path="url(#clip0_2_2)">
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M7.52944 7.02944C0.5 14.0589 0.5 25.3726 0.5 48V52C0.5 74.6274 0.5 85.9411 7.52944 92.9706C14.5589 100 25.8726 100 48.5 100H52.5C75.1274 100 86.4411 100 93.4706 92.9706C100.5 85.9411 100.5 74.6274 100.5 52V48C100.5 25.3726 100.5 14.0589 93.4706 7.02944C86.4411 0 75.1274 0 52.5 0H48.5C25.8726 0 14.5589 0 7.52944 7.02944ZM17.3752 30.4169C17.9168 56.4169 30.9167 72.0418 53.7084 72.0418H55.0003V57.1668C63.3753 58.0001 69.7082 64.1252 72.2498 72.0418H84.0835C80.8335 60.2085 72.2914 53.6668 66.9581 51.1668C72.2914 48.0835 79.7915 40.5835 81.5831 30.4169H70.8328C68.4995 38.6669 61.5836 46.1668 55.0003 46.8751V30.4169H44.2499V59.2501C37.5833 57.5835 29.1668 49.5002 28.7918 30.4169H17.3752Z"
                  fill="white"
                />
              </g>
              <defs>
                <clipPath id="clip0_2_2">
                  <rect
                    width="100"
                    height="100"
                    fill="white"
                    transform="translate(0.5)"
                  />
                </clipPath>
              </defs>
            </svg>
          </a>
        </li>
        <li class="icon-list icon-list-youtube">
          <a href="#" target="_blank" class="icon-text">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              xml:space="preserve"
              id="Layer_1"
              width="21"
              height="14"
              x="0"
              y="0"
              version="1.1"
              viewBox="0 0 71.412065 50"
            >
              <g id="g5" transform="scale(.58824)">
                <path
                  id="path7"
                  fill="#fff"
                  fill-opacity="1"
                  d="M35.705078 0S13.35386.0001149 7.765625 1.4707031c-3 .8235294-5.4713925 3.2946921-6.2949219 6.3535157C.0001149 13.412454 0 25 0 25s.0001149 11.64637 1.4707031 17.175781c.8235294 3.058824 3.2360984 5.471393 6.2949219 6.294922C13.412684 50.000115 35.705078 50 35.705078 50s22.353171-.000115 27.941406-1.470703c3.058824-.82353 5.471393-3.236098 6.294922-6.294922 1.470588-5.588235 1.470703-17.175781 1.470703-17.175781s.058709-11.64614-1.470703-17.2343752c-.823529-3.0588236-3.236098-5.4713925-6.294922-6.2949219C58.058249-.00011488 35.705078 0 35.705078 0zm-7.117187 14.294922L47.175781 25l-18.58789 10.705078V14.294922z"
                  transform="scale(1.7)"
                />
              </g>
            </svg>
          </a>
        </li>
      </ul>
      <img
        v-once
        src="../../assets/images/main.jpg"
        alt=""
        data-aos="fade-in"
      />
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

 <style id="style3" type="text/css">
.st0 {
  fill: red;
}
.st1 {
  fill: #fff;
}
.st2 {
  fill: #282828;
}
</style>