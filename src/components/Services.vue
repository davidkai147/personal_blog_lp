<template>
  <section class="services section" id="services">
    <h2 class="section__title">Services</h2>
    <span class="section__subtitle">What I offer</span>

    <div class="services__container container grid">
      <!-- Services 1 -->
      <div class="services__content">
        <div>
          <i class="uil uil-web-grid services__icon"></i>
          <h3 class="services__title">Website Development</h3>
        </div>

        <span
          class="button button--flex button--small button--link services__button"
        >
          View More
          <i class="uil uil-arrow-right button__icon"></i>
        </span>

        <div class="services__modal">
          <div class="services__modal-content">
            <h4 class="services__modal-title">Website Development</h4>
            <i class="uil uil-times services__modal-close"></i>

            <ul class="services__modal--services grid">
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  The website development process starts by taking the graphical
                  elements (colours, fonts, layout, images) defined in the
                  design process and coding them using web industry standards.
                </p>
              </li>
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  This is typically done by first coding the home page, followed
                  by templates for the interior pages.
                </p>
              </li>
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  When the website is ready for review you will be supplied with
                  login details to view the website before it is launched to the
                  public.
                </p>
              </li>
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  You will also be supplied with instructions on how to update
                  your website.
                </p>
              </li>
            </ul>
          </div>
        </div>
      </div>

      <!-- Services 2 -->
      <div class="services__content">
        <div>
          <i class="uil uil-shop services__icon"></i>
          <h3 class="services__title">eCommerce Solution</h3>
        </div>

        <span
          class="button button--flex button--small button--link services__button"
        >
          View More
          <i class="uil uil-arrow-right button__icon"></i>
        </span>

        <div class="services__modal">
          <div class="services__modal-content">
            <h4 class="services__modal-title">eCommerce Solution</h4>
            <i class="uil uil-times services__modal-close"></i>

            <ul class="services__modal--services grid">
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  An eCommerce solution is a feature-filled, customizable online
                  storefront and shopping cart that will be integrated into our
                  CMS.
                </p>
              </li>
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  The SSL certificate can be thought of as a lock-box for your
                  data. It doesn’t make it any harder for anyone to obtain the
                  data but it encrypts the data to the point that nobody can
                  understand it. In addition to encrypting data, the SSL
                  certificate ensures visitors that your business is legitimate,
                  and will not attempt to defraud them in any way.
                </p>
              </li>
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  An eCommerce payment gateway is a service that authorises your
                  customers’ credit card payments while processing them securely
                  with your merchant account.
                </p>
              </li>
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  When dealing with a payment gateway, you will also be required
                  to establish an online merchant account with your bank (fees
                  vary depending on the bank). We will be able to provide you
                  with information and instructions on how to establish a
                  merchant account once we know which bank you are using.
                </p>
              </li>
            </ul>
          </div>
        </div>
      </div>

      <!-- Services 3 -->
      <div class="services__content">
        <div>
          <i class="uil uil-mobile-android services__icon"></i>
          <h3 class="services__title">
            Mobile <br />
            Application
          </h3>
        </div>

        <span
          class="button button--flex button--small button--link services__button"
        >
          View More
          <i class="uil uil-arrow-right button__icon"></i>
        </span>

        <div class="services__modal">
          <div class="services__modal-content">
            <h4 class="services__modal-title">Mobile Application</h4>
            <i class="uil uil-times services__modal-close"></i>

            <ul class="services__modal--services grid">
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  The app design process starts with a pen and paper to sketch
                  page layouts, wire-frames, sitemaps and menu structures.
                </p>
              </li>
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  You will be presented with a variety of website design
                  concepts to review.
                </p>
              </li>
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  Feedback on the design concepts is essential to give you the
                  opportunity to express your thoughts on the design and make
                  alterations where desired before the final sign-off.
                </p>
              </li>
              <li class="services__modal-service">
                <i class="uil uil-check-circle services__modal-icon"></i>
                <p>
                  Once finalized, the design files will be supplied to you in
                  Figma and JPEG formats.
                </p>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  mounted() {
    /*==================== SERVICES MODAL ====================*/
    const modalViews = document.querySelectorAll(".services__modal"),
      modalBtns = document.querySelectorAll(".services__button"),
      modalCloses = document.querySelectorAll(".services__modal-close");

    let modal = function (modalClick) {
      modalViews[modalClick].classList.add("active-modal");
    };

    modalBtns.forEach((modalBtn, i) => {
      modalBtn.addEventListener("click", () => {
        modal(i);
      });
    });

    modalCloses.forEach((modalClose) => {
      modalClose.addEventListener("click", () => {
        modalViews.forEach((modalView) => {
          modalView.classList.remove("active-modal");
        });
      });
    });
  },
};
</script>