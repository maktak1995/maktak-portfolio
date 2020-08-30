<template>
  <SectionLayout icon="person-fill" title="Profile">
    <div class="profile-container">
      <img class="me" src="../../assets/maktak.jpg" />
      <div class="profile-content">
        <div class="h3">自己紹介</div>
        <p>
          はじめまして。私は牧田岳大(<a href="https://github.com/maktak1995"
            >@maktak1995</a
          >)と申します。
        </p>
        <p>
          大学で情報系の学科に進んだのをきっかけにプログラミングを始め、現在は株式会社VOYAGE
          GROUPにてフロントエンド関係のお仕事をやっています。
        </p>
        <p>
          主に使う言語はTypeScriptで、Reduxフレームワークを利用したアプリケーションの開発などをしています。
        </p>
        <div class="tech-stacks">
          <div class="h3">利用経験のある言語、FWなど</div>
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
}
.profile-content {
  text-align: left;
  padding-left: 32px;
  display: block;
}

.tech-stacks {
  padding-top: 18px;
}
.me {
  width: 250px;
  height: 250px;
  border-radius: 50%;
  background-position: center;
  background-size: cover;
}

.tech-icon {
  padding: 8px;
  height: 80px;
}
</style>
