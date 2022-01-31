<template>
  <SectionLayout icon="envelope" title="Contact">
    <div class="contact-container">
      <div class="h2 p-3 email">maktaktech@gmail.com</div>
      <div class="h3 p-4">OR</div>
      <a href="https://github.com/maktak1995">
        <img class="github" src="../../assets/github.png" />
      </a>
    </div>
  </SectionLayout>
</template>

<style>
.contact-container {
  width: 100%;
  display: flex;
  align-items: center;
  padding-bottom: 120px;
  @media screen and (max-width: 480px) {
    flex-direction: column;
  }
}
.email {
  background-color: #1e4270;
  color: whitesmoke;
}
.github {
  width: 70px;
}
</style>
