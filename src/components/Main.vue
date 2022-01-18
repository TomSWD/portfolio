<template>
  <div class="hero">
    <img class="background" src="@/assets/img/background.svg" />
    <div class="hero__container">
      <div class="hero__main">
        <h5 class="hero__title">Tomasz Swierad</h5>
        <h3 class="hero__sub-title">Junior Front-End Developer</h3>
        <a
          class="hero__btn"
          href="mailto:endurophine@gmail.com"
          subject="subject text"
          target="__blank"
          title="Tomasz Świerad e-mail"
          >Message Me</a
        >
      </div>
      <div class="hero__footer">
        <li class="hero__links">
          <ul>
            <a
              class="hero__link"
              href="https://drive.google.com/file/d/1j2KwZYamyAIzX-CdlcTH6Al1E6-BcOPi/view"
              target="__blank"
              title="Tomasz Świerad Resume"
              >Resume</a
            >
          </ul>
          <ul>
            <a
              class="hero__link"
              href="https://github.com/TomSWD"
              target="__blank"
              title="Tomasz Świerad GitHub"
              >Github</a
            >
          </ul>
          <ul>
            <a
              class="hero__link"
              href="https://www.linkedin.com/in/tomasz-swierad/"
              target="__blank"
              title="Tomasz Świerad LinkedIn"
              >LinkedIn</a
            >
          </ul>
          <ul>
            <a
              class="hero__link"
              href="https://calendly.com/tomswd"
              target="__blank"
              title="Tomasz Świerad Schedule a call"
              >Schedule a call</a
            >
          </ul>
        </li>
        <div class="hero__copyright">© 2021 Tomasz Świerad</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Main",
  components: {},
};
</script>

<style scoped>
.background {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.hero__container {
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  position: relative;
  max-width: 1480px;
  height: 100vh;
  margin: 0px auto;
  padding: 0px 20px 0px 20px;
}
.hero__main {
  max-width: 678px;
  width: 100%;
  margin: 0 auto;
  padding-top: 70px;
  display: flex;
  flex-direction: column;
  text-align: center;
  align-items: center;
}
.hero__title {
  font-size: 72px;
  font-weight: 900;
  line-height: 91px;
}
.hero__sub-title {
  font-size: 36px;
  font-weight: 400;
  line-height: 45px;
  padding-top: 10px;
}
.hero__btn {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 120px;
  height: 40px;
  background-color: #2f2f2f;
  border-radius: 8px;
  color: #fff;
  font-size: 14px;
  margin: 48px auto 0px;
}
.hero__btn:hover {
  opacity: 0.8;
  transition: 0.5s;
}
.hero__footer {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  margin-bottom: 30px;
  max-height: 200px;
  height: 100%;
}
.hero__links {
  display: flex;
  margin: auto;
  max-width: 536px;
  width: 100%;
  justify-content: space-between;
  font-size: 14px;
  line-height: 18px;
  font-weight: 400;
}
.hero__link:hover {
  transition: 0s;
  font-weight: 700;
}
.hero__copyright {
  font-size: 10px;
  margin: auto;
  margin: 0 auto;
}
@media (max-width: 707px) {
  .hero__main {
    padding-top: 50px;
  }
}
@media (max-width: 555px) {
  .hero__main {
    padding-top: 40px;
  }
  .hero__title {
    line-height: 70px;
  }
  .hero__title {
    font-size: 65px;
    line-height: 60px;
  }
  .hero__sub-title {
    font-size: 26px;
  }
  .hero__btn {
    margin: 40px auto 70px;
  }
}
@media (max-width: 480px) {
  .hero__btn {
    margin-bottom: 50px;
  }
  .hero__links {
    flex-direction: column;
    align-items: center;
    gap: 15px;
  }
  .hero__copyright {
    font-size: 8px;
    margin-top: 25px;
  }
}
</style>