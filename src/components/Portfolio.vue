<template>
  <section class="portfolio section" id="portfolio">
    <h2 class="section__title">Portfolio</h2>
    <span class="section__subtitle">Most recent work</span>

    <div class="portfolio__container container swiper-container">
      <div class="swiper-wrapper">
        <!-- Portfolio -->
        <div class="portfolio__content grid swiper-slide">
          <img
            src="../assets/img/portfolio1.jpg"
            alt=""
            class="portfolio__img"
          />
          <div class="portfolio__data">
            <h3 class="portfolio__title">Modern website</h3>
            <p class="portfolio__description">Coming soon...</p>
            <a
              href="#"
              class="button button--flex button--small portfolio__button"
            >
              Demo
              <i class="uil uil-arrow-right button__icon"></i>
            </a>
          </div>
        </div>

        <!-- Portfolio 2 -->
        <div class="portfolio__content grid swiper-slide">
          <img
            src="../assets/img/portfolio2.jpg"
            alt=""
            class="portfolio__img"
          />
          <div class="portfolio__data">
            <h3 class="portfolio__title">Modern website</h3>
            <p class="portfolio__description">Coming soon...</p>
            <a
              href="#"
              class="button button--flex button--small portfolio__button"
            >
              Demo
              <i class="uil uil-arrow-right button__icon"></i>
            </a>
          </div>
        </div>

        <!-- Portfolio 3 -->
        <div class="portfolio__content grid swiper-slide">
          <img
            src="../assets/img/portfolio3.jpg"
            alt=""
            class="portfolio__img"
          />
          <div class="portfolio__data">
            <h3 class="portfolio__title">Modern website</h3>
            <p class="portfolio__description">Coming soon...</p>
            <a
              href="#"
              class="button button--flex button--small portfolio__button"
            >
              Demo
              <i class="uil uil-arrow-right button__icon"></i>
            </a>
          </div>
        </div>
      </div>

      <!-- <div class="swiper-button-next">
        <i class="uil uil-angle-right-b swiper-portfolio-icon"></i>
      </div>
      <div class="swiper-button-prev">
        <i class="uil uil-angle-left-b swiper-portfolio-icon"></i>
      </div>
      <div class="swiper-pagination"></div> -->
    </div>
  </section>
</template>

<script>
import Swiper from "swiper/bundle";
// import Swiper styles
import "swiper/swiper-bundle.css";

export default {
  mounted() {
    // let swiperPortfolio = new Swiper(".portfolio__container", {
    //   autoplay: {
    //     delay: 5000,
    //   },
    //   cssMode: true,
    //   navigation: {
    //     nextEl: ".swiper-button-next",
    //     prevEl: ".swiper-button-prev",
    //   },
    //   pagination: {
    //     el: ".swiper-pagination",
    //   },
    // });
  },
};
</script>