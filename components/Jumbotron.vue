<template>
  <b-jumbotron
    header="MakTak's Portfolio"
    lead="This site is a portfolio-page of Takehiro Makita."
  >
    <p>このページは牧田岳大のポートフォリオサイトです。Nice to meet you !</p>
    <div class="menu">
      <IconLink link="#home" icon="house-fill" name="Home" />
      <IconLink link="#profile" icon="person-fill" name="Profile" />
      <IconLink link="#works" icon="code-slash" name="Works" />
      <IconLink link="#contact" icon="envelope" name="Contact" />
    </div>
  </b-jumbotron>
</template>

<style>
.jumbotron {
  background: url('~assets/topImg.jpg') center no-repeat;
  background-size: cover;
  background-color: rgba(167, 231, 255, 0.8);
  background-blend-mode: lighten;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 15%;
  width: 50%;
}
</style>
