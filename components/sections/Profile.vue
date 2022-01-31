<template>
  <SectionLayout icon="person-fill" title="Profile">
    <div class="profile-container">
      <div class="me" />
      <div class="profile-content">
        <p>
          はじめまして。牧田岳大(<a href="https://github.com/maktak1995"
            >@maktak1995</a
          >)と申します。
        </p>
        <p>
          大学で情報系の学科に進んだのをきっかけにプログラミングを始めました。
        </p>
        <p>
          現在は株式会社CARTAHOLDINGSにてWebサービスの開発業務を行っています。
        </p>
        <p>
          業務としてWebサービスの開発をフロントエンド・バックエンド問わず広範に行っていますが、<br />得意分野はフロントエンドです。
        </p>
        <div class="tech-stacks">
          <div class="h3">利用経験のある技術</div>
          <img class="tech-icon" src="../../assets/typeScript.png" />
          <img class="tech-icon" src="../../assets/react.png" />
          <img class="tech-icon" src="../../assets/redux.png" />
          <img class="tech-icon" src="../../assets/next.png" />
          <img class="tech-icon" src="../../assets/vue.png" />
          <img class="tech-icon" src="../../assets/nuxt-square.svg" />
          <img class="tech-icon" src="../../assets/marionette.png" />
          <img class="tech-icon" src="../../assets/python.png" />
          <img class="tech-icon" src="../../assets/gcp.png" />
          <img class="tech-icon" src="../../assets/firebase.png" />
          <img class="tech-icon" src="../../assets/aws.png" />
        </div>
      </div>
    </div>
  </SectionLayout>
</template>

<style>
.profile-container {
  width: 100%;
  display: flex;
  align-items: center;
  @media screen and (max-width: 480px) {
    flex-direction: column;
  }
}
.profile-content {
  text-align: left;
  padding-left: 32px;
  display: block;
  width: 80%;
  @media screen and (max-width: 480px) {
    padding-left: 0px;
    padding-top: 32px;
    width: 100%;
  }
}

.tech-stacks {
  padding-top: 18px;
}

.me {
  width: 250px;
  height: 250px;
  border-radius: 50%;
  background: center no-repeat;
  background-size: cover;
  background-image: url('../../assets/makitake.jpg');
}

.tech-icon {
  padding: 8px;
  height: 80px;
}
</style>
