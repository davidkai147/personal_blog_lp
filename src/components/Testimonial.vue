<template>
  <section class="testimonial section">
    <h2 class="section__title">Testimonial</h2>
    <span class="section__subtitle">My client saying</span>

    <div class="testimonial__container container swiper-container">
      <div class="swiper-wrapper">
        <!-- Testimonial 1 -->
        <div class="testimonial__content swiper-slide">
          <div class="testimonial__data">
            <div class="testimonial__header">
              <img
                src="../assets/img/testimonial1.jpg"
                alt=""
                class="testimonial__img"
              />

              <div>
                <h3 class="testimonial__name">Sara Smith</h3>
                <span class="testimonial__client">Client</span>
              </div>
            </div>

            <div>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
            </div>
          </div>

          <p class="testimonial__description">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nesciunt,
            iste quasi voluptatibus nemo totam molestiae aliquid vel excepturi
            asperiores necessitatibus exercitationem nobis adipisci hic amet qui
            voluptas tempora placeat perferendis!
          </p>
        </div>

        <!-- Testimonial 2 -->
        <div class="testimonial__content swiper-slide">
          <div class="testimonial__data">
            <div class="testimonial__header">
              <img
                src="../assets/img/testimonial2.jpg"
                alt=""
                class="testimonial__img"
              />

              <div>
                <h3 class="testimonial__name">Sara Smith</h3>
                <span class="testimonial__client">Client</span>
              </div>
            </div>

            <div>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
            </div>
          </div>

          <p class="testimonial__description">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nesciunt,
            iste quasi voluptatibus nemo totam molestiae aliquid vel excepturi
            asperiores necessitatibus exercitationem nobis adipisci hic amet qui
            voluptas tempora placeat perferendis!
          </p>
        </div>

        <!-- Testimonial 3 -->
        <div class="testimonial__content swiper-slide">
          <div class="testimonial__data">
            <div class="testimonial__header">
              <img
                src="../assets/img/testimonial3.jpg"
                alt=""
                class="testimonial__img"
              />

              <div>
                <h3 class="testimonial__name">Sara Smith</h3>
                <span class="testimonial__client">Client</span>
              </div>
            </div>

            <div>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
              <i class="uil uil-star testimonial__icon-star"></i>
            </div>
          </div>

          <p class="testimonial__description">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nesciunt,
            iste quasi voluptatibus nemo totam molestiae aliquid vel excepturi
            asperiores necessitatibus exercitationem nobis adipisci hic amet qui
            voluptas tempora placeat perferendis!
          </p>
        </div>
      </div>

      <div class="swiper-pagination swiper-pagination-testimonial"></div>
    </div>
  </section>
</template>

<script>
import Swiper from "swiper/bundle";
// import Swiper styles
import "swiper/swiper-bundle.css";

export default {
  mounted() {
    let swiperTestimonial = new Swiper(".testimonial__container", {
      loop: true,
      grabCursor: true,
      spaceBetween: 48,

      navigation: {
        nextEl: ".swiper-button-next",
        prevEl: ".swiper-button-prev",
      },
      pagination: {
        el: ".swiper-pagination",
        clickable: true,
        dynamicBullets: true,
      },
      breakpoints: {
        568: {
          slidesPerView: 2,
        },
      },
    });
  },
};
</script>