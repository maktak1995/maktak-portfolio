<template>
  <SectionLayout icon="code-slash" title="Works">
    <p>今まで私が開発したもの、開発をお手伝いしたものの一覧です。</p>
    <p>画像をクリックすると詳細が表示されます。</p>
    <div class="works-list">
      <div class="list-item">
        <ImageButtonModal image="portfolio.png" title="MakTak's Portfolio">
          <WorksContentLayout
            image="portfolio.png"
            source="https://github.com/maktak1995/maktak-portfolio"
          >
            このPortfolioサイトです。ページ自体はNuxt.jsで構築し、ページのホスティングにはAWSのサービス(S3,
            CloudFront, Certificate Manager, Route53)を利用しています。<br />
            ページ構成に悩みましたが、今回は簡潔で見やすいものにすることにフォーカスしました。
          </WorksContentLayout>
        </ImageButtonModal>
      </div>

      <div class="list-item">
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
      </div>
      <div class="list-item">
        <ImageButtonModal image="balus.png" title="BALUS">
          <WorksContentLayout
            image="balus.png"
            url="https://levii.co.jp/services/balus/trial/"
          >
            Model-based System Engineering
            を支援するコミュニケーションサービスです。様々な図を利用して上流設計や工程管理を行えるほか、図の同時編集やバージョン管理、メッセージによるコミュニケーション機能をもち、上流設計のためのGitHubといえるサービスです。<br />
            私はフロントエンドへの機能追加を主に担当しました。
          </WorksContentLayout>
        </ImageButtonModal>
      </div>
      <div class="list-item">
        <ImageButtonModal image="datastrap.png" title="DATA STRAP">
          <WorksContentLayout
            image="datastrap.png"
            url="https://lp.data-strap.com/"
          >
            複数のデマンドレポートや、計測ツールのデータを自動集計し、広告売上の管理・分析を効率化するサービスです。<br />
            DB設計、バックエンド開発、フロントエンド開発まで含めた新機能開発を担当しています。
          </WorksContentLayout>
        </ImageButtonModal>
      </div>
      <div class="list-item">
        <ImageButtonModal image="dreamkast.png" title="Dreamkast">
          <WorksContentLayout
            image="dreamkast.png"
            url="https://cloudnativedays.jp/"
            source="https://github.com/cloudnativedaysjp/dreamkast"
          >
            CloudNativeDaysというイベント向けに開発されたオンライン放送プラットフォームです。<br />
            私はUI設計、フロントエンド開発を担当しました。
          </WorksContentLayout>
        </ImageButtonModal>
      </div>
      <div class="list-item">
        <ImageButtonModal
          image="nijisanji-fanclub.png"
          title="にじさんじ FAN CLUB"
        >
          <WorksContentLayout
            image="nijisanji-fanclub.png"
            url="https://lp.data-strap.com/"
          >
            バーチャルライバー事務所「にじさんじ」に所属するタレントの公式ファンコミュニティサイトです。
            私はフロントエンドへの機能追加と保守を主に担当しました。
          </WorksContentLayout>
        </ImageButtonModal>
      </div>
    </div>
  </SectionLayout>
</template>

<style>
.works-list {
  padding-top: 32px;
  display: flex;
  justify-content: flex-start;
  flex-flow: row wrap;
  align-items: center;
  @media screen and (max-width: 480px) {
    flex-direction: column;
  }
}
.list-item {
  padding: 0px 0px 16px 16px;
}
</style>
