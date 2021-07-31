<template>
  <div>
    <div class="root">
      <div class="inner">
        <div>
          <img class="book" src="../assets/book_image@2x.png" />
        </div>
        <div class="contents">
          <div class="title">
            推しの話をきいて<br />全国推し菓子アンソロジー
          </div>
          <div class="product">
            A5サイズ / P108 / 特色2色刷り<br />
            頒布価格¥1000（＋送料180円）
          </div>
          <div class="description">
            「推し菓子を700文字で語って欲しい」<br />
            そんな思いつきツイートから始まったTwitterの祭り。
            100名以上を巻き込んで、ついに同人誌になりました！
            人の推しプレゼンは新しい出会いの扉、ピンときたらすぐにお試しあれ！公式通販の有無記載、公式サイトにすぐアクセスできるQRコード付き。
          </div>

          <div class="button-group">
            <br />
            <div class="button">
              <a href="https://ideots.booth.pm/items/3123134" target="_blank"
                >自家通販で購入</a
              >
            </div>
            <div class="button">
              <a href="https://ideots.booth.pm/items/3135221" target="_blank"
                >匿名配送で購入</a
              >
            </div>
            <!--
          <div class="button">
            <a href="https://ideots.booth.pm/items/3155209" target="_blank"
              >booth倉庫から購入</a
            >
          </div>-->
          </div>
        </div>
      </div>
    </div>
    <div class="pdf">
      <div class="box">
        <div class="sorry">お詫びと訂正</div>
        <br />
        <div class="text">
          先日頒布した『推しの話をきいて』初版・二刷に下記の訂正があります。
          <br />
          P42・P76に、和歌山「福菱 かげろう」の同じ原稿が掲載されていました。<br />
          P76の正しい原稿pdfを用意しましたので、お手数ですが印刷してご利用ください。
        </div>

        <div class="button02">
          <a href="https://oshi.174cm.com/pdf/p76.pdf" target="_blank"
            >pdfをダウンロード</a
          >
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
  @import "../assets/variable.scss";
  .pdf {
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding-bottom: 50px;
    > div {
      max-width: 680px;
    }
    .sorry {
      font-size: 1.5rem;
      font-weight: bold;
      @media screen and (max-width: 767px) {
        font-size: 1rem;
      }
    }
    .text {
      line-height: 1.7rem;
      @media screen and (max-width: 767px) {
        font-size: 0.8rem;
        line-height: 1.4rem;
      }
    }
    .box {
      justify-content: center;
      align-items: center;
      display: flex;
      flex-direction: column;
      padding: 20px;
      border: 2px solid #dcdcdc;
      text-align: center;
      border-radius: 10px;
      font-size: 18px;
    }
    .button02 {
      justify-content: center;
      align-items: center;
      text-align: center;
      font-size: 1rem;
      font-weight: bold;
      padding: 0.5rem 1rem;
      background-color: $primary;
      border-radius: 25px;
      width: 180px;
      margin-bottom: 1rem;
      margin-top: 1rem;

      > a {
        text-decoration: none;
        color: $secondary;
      }
    }
  }
  .root {
    background-color: $background;
    display: flex;
    justify-content: center;
    padding: 3rem 0;

    .inner {
      max-width: 680px;
      display: flex;
      justify-content: center;

      @media screen and (max-width: 767px) {
        flex-direction: column;
        align-items: center;
      }
    }

    .book {
      margin: 0 2rem;
      width: 280px;

      @media screen and (max-width: 320px) {
        width: 250px;
      }
    }

    .contents {
      @media screen and (max-width: 767px) {
        max-width: 400px;
        text-align: center;
      }

      .title {
        font-size: 1.4rem;
        font-weight: bold;
      }
      .product {
        padding-top: 0.5rem;
        font-size: 1rem;
        font-weight: bold;
      }
      .description {
        padding-top: 0.5rem;
        font-size: 0.8rem;
        line-height: 1.7;

        @media screen and (max-width: 767px) {
          padding-top: 2rem;
          padding: 1rem;
          max-width: 320px;
        }
      }

      .button-group {
        @media screen and (max-width: 767px) {
          display: flex;
          flex-direction: column;
          justify-content: center;
          align-items: center;
          width: 100%;
        }

        .button {
          text-align: center;
          font-size: 1rem;
          font-weight: bold;
          padding: 0.5rem 1rem;
          background-color: $primary;
          border-radius: 25px;
          width: 150px;
          margin-bottom: 1rem;

          > a {
            text-decoration: none;
            color: #000;
          }
        }
      }
    }
  }
</style>
