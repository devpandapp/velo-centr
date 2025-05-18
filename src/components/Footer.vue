<script setup lang="ts">
import { ref, onMounted, onUnmounted } from "vue";

const isVisible = ref<boolean>(false);

const handleScroll = () => {
  if (window.scrollY > 500) {
    isVisible.value = true;
  } else {
    isVisible.value = false;
  }
};

const scrollToTop = () => {
  window.scrollTo(0, 0);
};

onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});

onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>

<template>
  <div class="bottom-bg"></div>
  <footer class="footer-style">
    <div class="footer-top">
      <div class="container">
        <div class="row">
          <div class="col-lg-2 col-md-2">
            <div class="footer-widget widget">
              <div class="about_us_widget">
                <a href="index.html" class="logo d-flex align-items-center">
                  <h1 class="sitename">CENTR</h1>
                </a>
              </div>
            </div>
          </div>
          <div class="col-lg-6 col-md-6">
            <div class="navmenu footer-widget widget widget_nav_menu">
              <ul class="navmenu-list">
                <li class="item"><a class="link" href="#about">О нас</a></li>
                <li class="item">
                  <a class="link" href="#services">Секции</a>
                </li>
                <li class="item">
                  <a class="link" href="#schedule">Расписание</a>
                </li>
                <li class="item">
                  <a class="link" href="#schedule">Стоимость</a>
                </li>
                <li class="item">
                  <a class="link" href="#team">Команда</a>
                </li>
                <li class="item">
                  <a class="link" href="#contact">Контакты</a>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-lg-2 col-md-1">
            <div>
              <ul class="list-icons">
                <li>
                  <a
                    href="https://vk.com/centrschool63"
                    target="_blank"
                    class="icon-text icon-text-vk"
                  >
                    <svg
                      width="20"
                      height="19"
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
                  </a>
                </li>
                <li>
                  <a
                    href="#"
                    target="_blank"
                    class="icon-text icon-text-youtube"
                  >
                    <svg
                      width="26"
                      height="15"
                      viewBox="0 0 313.23315 216.02286"
                      version="1.1"
                      id="svg5"
                      xml:space="preserve"
                      xmlns="http://www.w3.org/2000/svg"
                      xmlns:svg="http://www.w3.org/2000/svg"
                    >
                      <defs id="defs2" />
                      <g
                        id="layer1"
                        transform="translate(-54.079375,-5.2758072)"
                      >
                        <path
                          d="m 210.53177,221.29866 c 0,0 98.12514,0 122.46443,-6.48069 13.70449,-3.6724 24.01093,-14.2575 27.62825,-27.32688 6.68807,-23.97854 6.68807,-74.41988 6.68807,-74.41988 0,0 0,-50.117297 -6.68807,-73.879819 C 357.00713,25.79798 346.70069,15.42887 332.9962,11.864515 308.65691,5.2758072 210.53177,5.2758072 210.53177,5.2758072 c 0,0 -97.9062,0 -122.135976,6.5887078 -13.485335,3.564355 -24.010529,13.933465 -27.847831,27.326876 -6.468588,23.762522 -6.468588,73.879819 -6.468588,73.879819 0,0 0,50.44134 6.468588,74.41988 3.837302,13.06938 14.362496,23.65448 27.847831,27.32688 24.229776,6.48069 122.135976,6.48069 122.135976,6.48069 z"
                          fill="#ff0033"
                          id="path1412"
                          style="stroke-width: 0.0208149"
                          clip-path="none"
                        />
                        <path
                          d="M 259.30109,113.28723 178.29251,67.382379 v 91.809711 z"
                          fill="#ffffff"
                          id="path1414"
                          style="stroke-width: 0.0208149"
                          clip-path="none"
                        />
                      </g>
                    </svg>
                  </a>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-lg-2 col-md-3 author">
            <a href="https://vk.com/aapand" target="_blank">© 2025 Pandapp</a>
          </div>
        </div>
      </div>
    </div>
  </footer>
  <div class="back-to-top" v-if="isVisible" @click="scrollToTop()">
    <span class="back-top"><i class="bi bi-chevron-up"></i></span>
  </div>
</template>

<style type="text/scss">
.footer-style {
  background: #efefef;

  .footer-top {
    background: #efefef;
    padding: 40px;

    .container {
      max-width: 97%;

      .logo {
        line-height: 1;
      }

      .sitename {
        font-size: 30px;
        margin: 0;
        font-weight: 700;
        font-style: italic;
        color: var(--heading-color);
      }

      .author {
        text-align: right;
        a {
          color: var(--heading-color);
          text-decoration: none;
        }
      }

      .list-icons {
        display: flex;
        list-style: none;

        .icon-text {
          font-size: 18px;
          padding: 0px 26px;
        }

        .icon-text-vk {
          color: var(--vk-color);
        }

        .icon-text-youtube {
          color: var(--youtube-color);
        }
      }

      .widget_nav_menu {
        .navmenu-list {
          padding: 0;

          .item {
            display: inline-block;
            margin: 0 !important;

            .link {
              color: var(--heading-color) !important;
              font-size: 18px;
              padding: 0px 26px;
              text-decoration: none;
            }

            @media only screen and (max-width: 1400px) {
              .link {
                padding: 0px 10px;
              }
            }

            .link:after {
              display: none;
            }

            .link:hover {
              color: var(--accent-color) !important;
            }
          }
        }
      }
    }
  }
}

.bottom-bg {
  background: url(../assets/images/footer.png);
  background-size: cover;
  min-height: 124px;
}

.back-to-top {
  position: fixed;
  right: 30px;
  bottom: 30px;
  width: 50px;
  height: 50px;
  color: var(--accent-color);
  background-color: #fff;
  text-align: center;
  border-radius: 50%;
  z-index: 99999;
  font-size: 34px;
  cursor: pointer;
  -webkit-box-shadow: 0 0 5px rgba(0, 0, 0, 0.5);
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.5);
}
</style>
