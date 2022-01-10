<template>
  <div class="hero">
    <img class="background" src="@/assets/img/background.svg" />
    <div class="hero__container">
      <a class="hero__website" href="#">swierad.pl</a>
      <div class="hero__main">
        <h5 class="hero__title">Tomasz Swierad</h5>
        <h3 class="hero__sub-title">Junior Front-End Developer</h3>
        <a class="hero__btn" href="#">Message Me</a>
      </div>
      <div class="hero__footer">
        <li class="hero__links">
          <ul>
            <a class="hero__link" href="#">Resume</a>
          </ul>
          <ul>
            <a class="hero__link" href="#">Github</a>
          </ul>
          <ul>
            <a
              class="hero__link"
              href="https://www.linkedin.com/in/tomasz-%C5%9Bwierad-573a1420b/"
              target="__blank"
              title="Tomasz Świerad LinkedIn"
              >LinkedIn</a
            >
          </ul>
          <ul>
            <a class="hero__link" href="#">Schedule a call</a>
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
  width: 100vw;
  /* height: 100vh; pierdoli*/
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

.hero__website {
  /* display: inline-block; ....jednak nie potrzebne?*/
  font-size: 14px;
  font-weight: 700;
  margin-top: 26px;
  margin-left: 64px;
}
.hero__website:hover {
  opacity: 0.8;
  transition: 0.3s;
}
.hero__main {
  max-width: 678px;
  /* margin-top: calc( - 244px); */
  margin: auto;
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
  width: 113px;
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
  width: 50%;
}
.hero__footer {
  display: flex;
  flex-direction: column;
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
  margin: 86px auto 16px;
}
@media (max-width: 707px) {
  .hero__title {
    line-height: 70px;
  }
}
@media (max-width: 555px) {
  .hero__main {
    padding-top: 20px;
  }
  .hero__title {
    font-size: 65px;
    line-height: 60px;
  }
  .hero__sub-title {
    font-size: 26px;
  }
  .hero__btn {
    margin: 40px auto 100px;
    width: 100%;
  }
}
@media (max-width: 555px) {
  .hero__title {
    font-size: 55px;
    line-height: 60px;
  }
  .hero__sub-title {
    font-size: 26px;
  }
}
@media (max-width: 480px) {
  /* .hero__website {
    margin-top: 90px;
  } */
  .hero__btn {
    margin-bottom: 40px;
  }
  .hero__links {
    flex-direction: column;
    align-items: center;
    gap: 15px;
  }
  .hero__copyright {
    font-size: 8px;
    margin-top: 45px;
  }
}
</style>