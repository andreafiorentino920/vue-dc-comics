<template>
  <div>
    <header>
      <Header/>
    </header>
    <main>
      <Section1/>
      <Section2/>>
    </main>
    <footer>
      <FooterTop/>
      <FooterBottom/>
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Section1 from './components/Section1.vue'
import Section2 from './components/Section2.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'

export default {
  components: {
    Header,
    Section1,
    Section2,
    FooterTop,
    FooterBottom


  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=PT+Sans+Narrow:wght@400;700&display=swap');
body{
  font-family: 'PT Sans Narrow', sans-serif;
}
</style>
