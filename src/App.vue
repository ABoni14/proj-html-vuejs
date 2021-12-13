<template>
  <div>
    <Header />
    <JumboTron />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue"
import JumboTron from "./components/JumboTron.vue"
import Main from "./components/Main.vue"
import Footer from "./components/Footer.vue"

export default {
  name: 'App',
  components: {
    Header,
    JumboTron,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import "./assets/style/vars.scss";
@import "./assets/style/utilities.scss";
@import "./assets/style/generals.scss"

</style>
