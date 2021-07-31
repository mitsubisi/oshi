<template>
  <div class="root">
    <div class="inner">
      <div class="triangle">
        <div />
      </div>
      <div class="box">
        <div class="image-box">
          <span class="title">ピックアップ推し菓子 </span>
          <div>
            <img class="image" src="../assets/book_illust@2x.png" />
          </div>
        </div>
        <div class="description">
          <div class="prefecture">新潟</div>
          <div class="name">明治屋 ゆか里/浮き星</div>
          <p class="text">
            見た目はまるで金平糖、だけどその正体は砂糖蜜をかけた「あられ」。お湯やお茶に浮かせるのもいいし、そのままぽりぽり食べても美味しい魅惑のお菓子！
            <br />
            新潟が誇る銘菓なのに、後継者がいない！？どうなっちゃうの…！？なんとデザインと名前をリニューアル、かわいいお菓子がさらにキュートになったのです！
            <br />
            カラフルな色だけでしょ、って？いいえ、フレーバーはなんと15種類！お好みの味をぜひ試してみてくださいね。
          </p>
          <p class="text">
            参考サイト<br />
            日刊にいがたwebタウン情報<br />

            <a href="https://tjniigata.jp/gourmet/202102yukari/" target="_blank"
              >https://tjniigata.jp/gourmet/202102yukari/</a
            ><br /><br />
            浮き星（オンラインショップあり、ミニ袋302円〜）<br />
            <a href="http://ukihoshi.com/" target="_blank"
              >http://ukihoshi.com/</a
            ><br />
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
@import "../assets/variable.scss";

.root {
  background-color: $primary;
  display: flex;
  justify-content: center;
  padding: 1rem 0 3rem 0;

  @media screen and (max-width: 767px) {
    padding-bottom: 1rem;
  }

  .inner {
    width: 800px;

    @media screen and (max-width: 767px) {
      max-width: 480px;
    }
  }

  .triangle {
    display: flex;
    justify-content: center;

    > div {
      width: 0px;
      border-right: 50px solid transparent;
      border-bottom: 50px solid $background;
      border-left: 50px solid transparent;
    }
  }

  .box {
    display: flex;
    width: 100%;
    background-color: $background;
    padding: 0.75rem 0 0 0;

    @media screen and (max-width: 767px) {
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    .image-box {
      .title {
        background-color: $secondary;
        color: $background;
        padding: 0 0.5rem;
      }

      .image {
        padding: 1rem;
        width: 400px;

        @media screen and (max-width: 767px) {
          max-width: 300px;
        }

        @media screen and (max-width: 320px) {
          max-width: 280px;
        }
      }
    }

    .description {
      width: 400px;

      @media screen and (max-width: 767px) {
        max-width: 300px;
      }

      @media screen and (max-width: 320px) {
        max-width: 280px;
      }

      padding: 1rem;

      .prefecture {
        font-size: 1.2rem;
        font-weight: bold;
        line-height: 1;
      }

      .name {
        font-size: 1.5rem;
        font-weight: bold;
      }

      .text {
        font-size: 0.75rem;
        line-height: 1.6;
      }
    }
  }
}
</style>
