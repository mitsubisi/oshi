<template>
  <div class="root">
    <div class="inner">
      主催：ideots（ミツビシ）<br />
      このページは同人誌「推しの話をきいて」の告知ページです。<br />
      個人が趣味で作ったものであり、いかなる会社とも関係ありません。<br />
      お問い合わせはメールフォームからお願いします。返信までお時間をいただくことがあります。<br />
    </div>
  </div>
</template>

<style scoped lang="scss">
@import "../assets/variable.scss";

.root {
  background-color: $primary;
  display: flex;
  justify-content: center;
  padding-top: 2rem;
  padding-bottom: 5rem;

  .inner {
    width: 680px;
    text-align: left;
    font-weight: bold;
    font-size: 0.75rem;
    line-height: 1.6;

    @media screen and (max-width: 767px) {
      padding: 0 1rem;
      font-size: 0.5rem;
      line-height: 1.6;
    }
  }
}
</style>
