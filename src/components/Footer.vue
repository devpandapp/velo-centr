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
                    href="https://vk.com/malyaevbmx"
                    target="_blank"
                    class="icon-text icon-text-vk"
                  >
                    <i class="bi bi-vimeo"></i>
                  </a>
                </li>
                <li>
                  <a
                    href="#"
                    target="_blank"
                    class="icon-text icon-text-youtube"
                  >
                    <i class="bi bi-youtube"></i>
                  </a>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-lg-2 col-md-3 author">
            <a href="https://vk.com/aapand" target="_blank">© 2024 Pandapp</a>
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
