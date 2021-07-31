<template>
  <div class="root">
    <div class="book-images">
      <img class="image1" src="../assets/header_illust01@2x.png" />
      <img class="image2" src="../assets/header_illust02@2x.png" />
      <img class="image3" src="../assets/header_illust03@2x.png" />
      <img class="image4" src="../assets/header_illust04@2x.png" />
      <img class="image5" src="../assets/header_illust05@2x.png" />
      <img class="image6" src="../assets/header_illust06@2x.png" />
      <img class="image7" src="../assets/header_illust07@2x.png" />
      <img class="image8" src="../assets/header_illust08@2x.png" />
    </div>
    <div class="title">
      <div>推しの</div>
      <div class="center">
        話を
        <div class="sub">全国の推し菓子<br />アンソロジー</div>
      </div>
      <div>きいて</div>
    </div>
    <div class="heading">
      <div>
        <span class="text">星<span>の</span>数<span>なんて</span>関係ない､</span
        ><br /><span class="text"
          >これ<span>が</span>私<span>の</span>推し菓子！</span
        >
      </div>
    </div>
    <div class="description">
      <div>
        ほとばしる郷土愛、旅行の記憶、<br />青春の思い出、家族の好物ーー。<br />お菓子と人生が交わる時、<br />そこにはうつくしい物語の旋律が生まれる。<br /><br />
        総勢<span>94名</span>による700文字の熱いプレゼン、<br />集まった推し菓子総数なんと<span>200</span>件超え！<br />
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
@import "../assets/variable.scss";

.root {
  position: relative;
  background-image: url("../assets/header_bg@2x.png");
  background-size: contain;
  background-position: top;
  background-color: $primary;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 2rem 2rem 5rem 2rem;
  background-repeat: no-repeat;

  @media screen and (min-width: 1300px) {
    background-size: 1400px;
  }

  @media screen and (max-width: 767px) {
    background-size: 1000px;
  }
}

.book-images {
  position: relative;
  min-width: 980px;

  @media screen and (max-width: 767px) {
    display: none;
  }

  .image1 {
    position: absolute;
    width: 200px;
    top: 6rem;
    right: 5rem;
    opacity: 0;
    animation: fadein-anim 1.5s linear forwards;
    animation-delay: 0s;
  }
  .image2 {
    position: absolute;
    width: 200px;
    top: 6rem;
    left: 5rem;
    opacity: 0;
    animation: fadein-anim 1.5s linear forwards;
    animation-delay: 0.75s;
  }
  .image3 {
    position: absolute;
    width: 200px;
    top: 18rem;
    right: 12rem;
    opacity: 0;
    animation: fadein-anim 1.5s linear forwards;
    animation-delay: 1.5s;
  }
  .image4 {
    position: absolute;
    width: 200px;
    top: 18rem;
    left: 10rem;
    opacity: 0;
    animation: fadein-anim 1.5s linear forwards;
    animation-delay: 2.25s;
  }
  .image5 {
    position: absolute;
    width: 200px;
    top: 30rem;
    right: 6rem;
    opacity: 0;
    animation: fadein-anim 1.5s linear forwards;
    animation-delay: 3s;
  }
  .image6 {
    position: absolute;
    width: 200px;
    top: 30rem;
    left: 4rem;
    opacity: 0;
    animation: fadein-anim 1.5s linear forwards;
    animation-delay: 3.75s;
  }
  .image7 {
    position: absolute;
    width: 200px;
    top: 40rem;
    right: 8rem;
    opacity: 0;
    animation: fadein-anim 1.5s linear forwards;
    animation-delay: 4.5s;
  }
  .image8 {
    position: absolute;
    width: 225px;
    top: 40rem;
    left: 6rem;
    opacity: 0;
    animation: fadein-anim 2s linear forwards;
    animation-delay: 5.25s;
  }
}

@keyframes fadein-anim {
  100% {
    opacity: 1;
  }
}

.title {
  -webkit-writing-mode: vertical-rl;
  -ms-writing-mode: tb-rl;
  writing-mode: vertical-rl;
  line-height: 1.1;

  font-size: 6rem;
  font-weight: bold;
  color: $secondary;

  @media screen and (max-width: 320px) {
    font-size: 5.5rem;
  }

  .center {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;

    .sub {
      background-color: $background;
      font-size: 1.6rem;
      font-weight: bold;
      color: $secondary;
      margin-top: 1rem;
      padding: 0.75rem;
    }
  }
}

.heading {
  padding-top: 3rem;
  font-size: 2rem;
  font-weight: bold;
  color: $secondary;
  line-height: 1.6;
  text-align: center;

  @media screen and (max-width: 320px) {
    font-size: 1.5rem;
  }

  .text {
    background-color: $background;

    span {
      font-size: 1.6rem;

      @media screen and (max-width: 320px) {
        font-size: 1.2rem;
      }
    }
  }
}

.description {
  padding-top: 2rem;
  font-weight: bold;
  text-align: center;
  font-size: 0.9rem;

  span {
    color: $secondary;
  }
}
</style>
