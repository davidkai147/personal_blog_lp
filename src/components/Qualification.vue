<template>
  <section class="qualification section">
    <h2 class="section__title">Qualifications</h2>
    <span class="section__subtitle">My personal journey</span>

    <div class="qualification__container container">
      <div class="qualification__tabs">
        <div
          class="qualification__button button--flex qualification__active"
          data-target="#education"
        >
          <i class="uil uil-graduation-cap qualification__icon"></i>
          Education
        </div>

        <div class="qualification__button button--flex" data-target="#work">
          <i class="uil uil-briefcase-alt qualification__icon"></i>
          Work
        </div>
      </div>

      <div class="qualification__sections">
        <!-- Qualification content 1 -->
        <div
          class="qualification__content qualification__active"
          data-content
          id="education"
        >
          <!-- Qualification 1 -->
          <div class="qualification__data">
            <div>
              <h3 class="qualification__title">Computer Science</h3>
              <span class="qualification__subtitle"
                >Greenwich - University</span
              >
              <div class="qualification__calendar">
                <i class="uil uil-calendar-alt"></i>
                2010 - 2013
              </div>
            </div>

            <div>
              <span class="qualification__rounder"></span>
              <span class="qualification__line"></span>
            </div>
          </div>
          <!-- Qualification 2 -->
          <div class="qualification__data">
            <div></div>
            <div>
              <span class="qualification__rounder"></span>
            </div>
          </div>
        </div>

        <!-- Qualification content 2 -->
        <div class="qualification__content" data-content id="work">
          <!-- Qualification 2 -->
          <div class="qualification__data">
            <div>
              <h3 class="qualification__title">FSS</h3>
              <span class="qualification__subtitle">Web Developer</span>
              <div class="qualification__calendar">
                <i class="uil uil-calendar-alt"></i>
                2013 - 2015
              </div>
            </div>

            <div>
              <span class="qualification__rounder"></span>
              <span class="qualification__line"></span>
            </div>
          </div>

          <div class="qualification__data">
            <div></div>
            <div>
              <span class="qualification__rounder"></span>
              <span class="qualification__line"></span>
            </div>
            <div>
              <h3 class="qualification__title">NTT Data</h3>
              <span class="qualification__subtitle">Web Developer</span>
              <div class="qualification__calendar">
                <i class="uil uil-calendar-alt"></i>
                2015 - 2017
              </div>
            </div>
          </div>

          <div class="qualification__data">
            <div>
              <h3 class="qualification__title">Gonosen</h3>
              <span class="qualification__subtitle"
                >Full-stack Web Developer</span
              >
              <div class="qualification__calendar">
                <i class="uil uil-calendar-alt"></i>
                2018 - 2020
              </div>
            </div>

            <div>
              <span class="qualification__rounder"></span>
              <span class="qualification__line"></span>
            </div>
          </div>

          <div class="qualification__data">
            <div></div>
            <div>
              <span class="qualification__rounder"></span>
              <span class="qualification__line"></span>
            </div>
            <div>
              <h3 class="qualification__title">Gumi Vietnam</h3>
              <span class="qualification__subtitle"
                >Full-stack Web Developer</span
              >
              <div class="qualification__calendar">
                <i class="uil uil-calendar-alt"></i>
                2020 - Now
              </div>
            </div>
          </div>

          <div class="qualification__data">
            <div></div>
            <div>
              <span class="qualification__rounder"></span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  mounted() {
    /*==================== QUALIFICATION TABS ====================*/
    const tabs = document.querySelectorAll("[data-target]"),
      tabContents = document.querySelectorAll("[data-content]");

    tabs.forEach((tab) => {
      tab.addEventListener("click", () => {
        const target = document.querySelector(tab.dataset.target);

        tabContents.forEach((tabContent) => {
          tabContent.classList.remove("qualification__active");
        });

        target.classList.add("qualification__active");

        tabs.forEach((tab) => {
          tab.classList.remove("qualification__active");
        });

        tab.classList.add("qualification__active");
      });
    });
  },
};
</script>