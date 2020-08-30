<template>
  <SectionLayout icon="code-slash" title="Works">
    <p>今まで私が開発したもの、開発をお手伝いしたものの一覧です。</p>
    <p>画像をクリックすると詳細が表示されます。</p>
    <div class="works-list">
      <ImageButtonModal image="portfolio.png" title="MakTak's Portfolio">
        <WorksContentLayout
          image="portfolio.png"
          url="https://maktak.tk/"
          source="https://github.com/maktak1995/maktak-portfolio"
        >
          このPortfolioサイトです。ページ自体はNuxt.jsで構築し、ページのホスティングにはAWSのサービス(S3,
          CloudFront, Certificate Manager, Route53)を利用しています。<br />
          ページ構成に悩みましたが、今回は簡潔で見やすいものにすることにフォーカスしました。
        </WorksContentLayout>
      </ImageButtonModal>

      <ImageButtonModal image="datastore-viewer.png" title="Datastore Viewer">
        <WorksContentLayout
          image="datastore-viewer.png"
          source="https://github.com/gumo-py/datastore-viewer"
        >
          Google App
          Engineの第２世代をローカルの端末で検証を行うためのDBビューワーです。
          アプリの詳細な仕様や開発の目的については<a
            href="https://blog.levii.co.jp/entry/datastore-viewer-release"
            >このブログ記事</a
          >にまとまっていますので、こちらもご確認いただければと思います。<br />
          私はフロントエンドの設計と開発、バックエンドのAPI実装を担当しました。フロントに関してはReact
          + Material-UIで開発しています。
        </WorksContentLayout>
      </ImageButtonModal>

      <ImageButtonModal image="balus.jpg" title="BALUS">
        <WorksContentLayout image="balus.jpg" url="https://app.balus.me/">
          Model-based System Engineering
          を支援するコミュニケーションサービスです。様々な図を利用して上流設計や工程管理を行えるほか、図の同時編集やバージョン管理、メッセージによるコミュニケーション機能をもち、さしづめ上流設計のためのGitHubといえるサービスです。<br />
          バックエンドはGCPにより構築されており、フロントエンドはES6、フレームワークにBackbone.Marionetteを利用して構築されています。<br />
          私はフロントエンドへの機能追加を主に担当しました。
        </WorksContentLayout>
      </ImageButtonModal>

      <ImageButtonModal image="datastrap.png" title="DATA STRAP">
        <WorksContentLayout
          image="datastrap.png"
          url="https://data-strap.com/lp"
        >
          複数のデマンドレポートや、計測ツールのデータを自動集計し、広告売上の管理・分析を効率化するサービスです。バックエンドはAWSで管理されており、フロントエンドはReduxで構築されています。<br />
          私はフロントエンドへの機能設計や追加を主に担当しています。
        </WorksContentLayout>
      </ImageButtonModal>
    </div>
  </SectionLayout>
</template>

<style>
.works-list {
  padding-top: 32px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 70vw;
}
</style>
