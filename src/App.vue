<template>
  <div id="app">
    <Top />
    <Book />
    <PickUp />
    <Detail />
    <Report />
    <Footer />
  </div>
</template>

<script>
  import Top from "./components/Top.vue";
  import Book from "./components/Book.vue";
  import PickUp from "./components/PickUp.vue";
  import Detail from "./components/Detail.vue";
  import Report from "./components/Report.vue";
  import Footer from "./components/Footer.vue";

  export default {
    name: "App",
    components: {
      Top,
      Book,
      PickUp,
      Detail,
      Report,
      Footer,
    },
  };
</script>

<style lang="scss">
  #app {
    font-family: "Noto Sans JP", sans-serif;
  }

  body {
    margin: 0;
  }
</style>
