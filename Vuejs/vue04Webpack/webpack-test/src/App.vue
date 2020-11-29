
<style scoped>
section {
  height: 150px;
  background-color: #95db5e;
  margin: 0 5% 20px 5%;
  margin: 40px 0px;
}

div {margin: 40px 20px;}
</style>

<template>
  <div class="container">
    <header-comp></header-comp>

    <section id="page1" data-role="page">
        <div class="content" data-role="content">컨텐츠</div>
    </section>

    <footer-comp></footer-comp>
  </div>
</template>

<script>
import Header from "./Header.vue"; //파일불러오기
import Footer from "./Footer.vue"; //파일불러오기

export default {
  data() {
    return {
      msg: "Hello VueJS",
    };
  },
  components: {
    "header-comp": Header, //파일결합
    "footer-comp": Footer, //파일결합
  },
};
</script>
