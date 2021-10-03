<template>
  <div>
    <header>
      <Header/>
    </header>
    <main>
      <Hero :bgImage="require('./assets/jumbotron.jpg')"/>
      <Section1/>
      <Section2/>
    </main>
    <footer>
      <FooterTop/>
      <FooterBottom/>
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Section1 from './components/Section1.vue'
import Section2 from './components/Section2.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'


export default {
  components: {
    Header,
    Hero,
    Section1,
    Section2,
    FooterTop,
    FooterBottom
  }
}
</script>

<style lang="scss">
@import "./assets/sass/common.scss";
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.padding{
  padding-left: 150px;
}
</style>
