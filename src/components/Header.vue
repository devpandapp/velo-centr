<template>
  <header id="header" class="header d-flex align-items-center fixed-top">
    <div
      class="container-fluid container-xl position-relative d-flex align-items-center justify-content-between"
    >
      <a href="index.html" class="logo d-flex align-items-center">
        <h1 class="sitename">CENTR</h1>
      </a>
      <nav class="navbar navbar-expand-lg">
        <div class="container-fluid">
          <div class="navbar-toggler dropstart">
            <a
              class="dropdown-menu-button"
              href="#"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              <i class="bi bi-justify-right"></i>
            </a>
            <ul class="dropdown-menu">
              <li>
                <a class="dropdown-item" href="#about">О нас</a>
              </li>
              <li>
                <a class="dropdown-item" href="#services">Секции</a>
              </li>
              <li>
                <a class="dropdown-item" href="#schedule">Расписание</a>
              </li>
              <li>
                <a class="dropdown-item" href="#schedule">Стоимость</a>
              </li>
              <li>
                <a class="dropdown-item" href="#team">Команда</a>
              </li>
              <li>
                <a class="dropdown-item" href="#contact">Контакты</a>
              </li>
            </ul>
          </div>
          <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
            <ul class="navbar-nav">
              <li class="nav-link"><a href="#about">О нас</a></li>
              <li class="nav-link"><a href="#services">Секции</a></li>
              <li class="nav-link"><a href="#schedule">Расписание</a></li>
              <li class="nav-link"><a href="#schedule">Стоимость</a></li>
              <li class="nav-link"><a href="#team">Команда</a></li>
              <li class="nav-link"><a href="#contact">Контакты</a></li>
            </ul>
          </div>
        </div>
      </nav>
    </div>
  </header>
</template>

<style type="text/scss">
.header {
  --background-color: rgba(0, 0, 0, 0);
  --default-color: #ffffff;
  --heading-color: #ffffff;
  color: var(--default-color);
  background-color: var(--background-color);
  padding: 15px 0;
  transition: all 0.5s;
  z-index: 997;
  position: absolute !important;

  .logo {
    line-height: 1;

    h1 {
      font-size: 30px;
      margin: 0;
      font-weight: 700;
      font-style: italic;
      color: var(--heading-color);
    }
  }

  .navbar-toggler {
    border: 0;
    padding: 0;

    .dropdown-menu {
      min-width: inherit;
      background-color: var(--accent-color);

      .dropdown-item {
        color: var(--default-color);
      }
    }

    .dropdown-menu-button {
      color: var(--default-color);
      font-size: 2rem;
    }
  }
}
</style>
