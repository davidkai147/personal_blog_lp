<template>
  <div class="layout">
    <header class="header" id="header">
    <nav class="nav container">
      <a href="#" class="nav__logo">congdo.dev</a>

      <div class="nav__menu" id="nav-menu">
        <ul class="nav__list grid">
          <li class="nav__item">
            <a href="#home" class="nav__link active-link">
              <i class="uil uil-estate nav__icon"></i> Home
            </a>
          </li>
          <li class="nav__item">
            <a href="#about" class="nav__link">
              <i class="uil uil-user nav__icon"></i> About
            </a>
          </li>
          <li class="nav__item">
            <a href="#skills" class="nav__link">
              <i class="uil uil-file-alt nav__icon"></i> Skills
            </a>
          </li>
          <li class="nav__item">
            <a href="#services" class="nav__link">
              <i class="uil uil-briefcase-alt nav__icon"></i> Services
            </a>
          </li>
          <li class="nav__item">
            <a href="#portfolio" class="nav__link">
              <i class="uil uil-scenery nav__icon"></i> Portfolio
            </a>
          </li>
          <li class="nav__item">
            <a href="#portfolio" class="nav__link">
              <i class="uil uil-document-layout-center nav__icon"></i> Blog
            </a>
          </li>
          <li class="nav__item">
            <a href="#contact" class="nav__link">
              <i class="uil uil-message nav__icon"></i> Contact me
            </a>
          </li>
        </ul>
        <i class="uil uil-times nav__close" id="nav-close"></i>
      </div>

      <div class="nav__btns">
        <!-- sTheme change button -->
        <i class="uil uil-moon change-theme" id="theme-button"></i>
        <div class="nav__toggle" id="nav-toggle">
          <i class="uil uil-apps"></i>
        </div>
      </div>
    </nav>
  </header>
  <main class="main">
    <slot/>
  </main>
<!--==================== FOOTER ====================-->
  <footer class="footer">
    <div class="footer__bg">
      <div class="footer__container container grid">
        <div>
          <h1 class="footer__title">Công Đỗ</h1>
          <span class="footer__subtitle">A passionate full-stack web & mobile developer</span>
        </div>

        <ul class="footer__links">
          <li>
            <a href="#services" class="footer__link">Services</a>
          </li>
          <li>
            <a href="#portfolio" class="footer__link">Portfolio</a>
          </li>
          <li>
            <a href="#contact" class="footer__link">Contact</a>
          </li>
        </ul>

        <div class="footer__socials">
          <a href="https://www.linkedin.com/in/congdct/" target="_blank" class="footer__social">
            <i class="uil uil-linkedin-alt"></i>
          </a>
          <a href="https://facebook.com/davidkai147" target="_blank" class="footer__social">
            <i class="uil uil-facebook-f"></i>
          </a>
          <a href="https://github.com/davidkai147" target="_blank" class="footer__social">
            <i class="uil uil-github-alt"></i>
          </a>
          <a href="https://instagram.com/davidkai_jm" target="_blank" class="footer__social">
            <i class="uil uil-instagram"></i>
          </a>
        </div>
      </div>

      <p class="footer__copy">&#169; congdo.dev. All right reserved. Tutorial by Bedimcode</p>
    </div>
  </footer>
  <!--==================== SCROLL TOP ====================-->
  <a href="#" class="scrollup" id="scroll-up">
    <i class="uil uil-arrow-up scrollup__icon"></i>
  </a>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>
<style>
@import 'https://unicons.iconscout.com/release/v4.0.0/css/line.css';
</style>