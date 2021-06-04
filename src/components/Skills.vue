<template>
  <section class="skills section" id="skills">
    <h2 class="section__title">Skills</h2>
    <span class="section__subtitle">My technical level</span>

    <div class="skills__container container grid">
      <div>
        <!-- SKILL 1-->
        <div class="skills__content skills__open">
          <div class="skills__header">
            <i class="uil uil-brackets-curly skills__icon"></i>

            <div>
              <h1 class="skills__title">Backend</h1>
              <span class="skills__subtitle">More than 6 years</span>
            </div>
          </div>

          <div class="skills__list grid">
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">Laravel</h3>
                <span class="skills__number">5 years</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__html"></span>
              </div>
            </div>

            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">NodeJS</h3>
                <span class="skills__number">5 years</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__css"></span>
              </div>
            </div>

            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">Golang</h3>
                <span class="skills__number">1 year</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__js"></span>
              </div>
            </div>
          </div>
        </div>

        <!-- SKILL 2-->
        <div class="skills__content skills__open">
          <div class="skills__header">
            <i class="uil uil-server-network skills__icon"></i>

            <div>
              <h1 class="skills__title">Mobile</h1>
              <span class="skills__subtitle">More than 2 years</span>
            </div>
          </div>

          <div class="skills__list grid">
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">Android (Kotlin)</h3>
                <span class="skills__number">2 years</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__html"></span>
              </div>
            </div>

            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">iOS</h3>
                <span class="skills__number">6 months</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__css"></span>
              </div>
            </div>

            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">Flutter</h3>
                <span class="skills__number">1 year</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__js"></span>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div>
        <!-- SKILL 4 -->
        <div class="skills__content skills__open">
          <div class="skills__header">
            <i class="uil uil-server-network skills__icon"></i>

            <div>
              <h1 class="skills__title">Frontend</h1>
              <span class="skills__subtitle">More than 6 years</span>
            </div>
          </div>

          <div class="skills__list grid">
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">HTML & CSS</h3>
                <span class="skills__number">6 years</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__html"></span>
              </div>
            </div>

            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">JavaScript</h3>
                <span class="skills__number">6 years</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__js"></span>
              </div>
            </div>

            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">VueJS</h3>
                <span class="skills__number">2 years</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__react"></span>
              </div>
            </div>
          </div>
        </div>

        <div class="skills__content skills__open">
          <div class="skills__header">
            <i class="uil uil-server-network skills__icon"></i>

            <div>
              <h1 class="skills__title">Database & Tool</h1>
              <span class="skills__subtitle">More than 6 years</span>
            </div>
          </div>

          <div class="skills__list grid">
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">MySQL</h3>
                <span class="skills__number">6 years</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__html"></span>
              </div>
            </div>

            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">PostgreSQL</h3>
                <span class="skills__number">2 years</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__js"></span>
              </div>
            </div>

            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">MongoDB</h3>
                <span class="skills__number">2 years</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__react"></span>
              </div>
            </div>

            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">VS Code</h3>
                <span class="skills__number">3 years</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__react"></span>
              </div>
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
    /*==================== ACCORDION SKILLS ====================*/
    const skillsContent = document.getElementsByClassName("skills__content"),
      skillsHeader = document.querySelectorAll(".skills__header");

    function toggleSkills() {
      let itemClass = this.parentNode.className;

      for (i = 0; i <= skillsContent.length; i++) {
        skillsContent[i].className = "skills__content skills__close";
      }

      if (itemClass === "skills__content skills__close") {
        this.parentNode.className = "skills__content skills__open";
      }
    }

    skillsHeader.forEach((el) => {
      el.addEventListener("click", toggleSkills);
    });
  },
};
</script>