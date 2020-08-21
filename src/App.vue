<template>
  <div id="app">
    <Header></Header>
    <Slider></Slider>
    <About></About>
    <News></News>
    <Subscribe></Subscribe>
    <Footer></Footer>
  </div>
</template>

<style lang="scss">
  @import "style/global.scss";
  @import "components/slider/vueperslide";

</style>
<script>
import Header from './components/header/Header'
import Slider from './components/slider/Slider'
import About from './components/about/About'
import News from './components/news/News'
import Footer from './components/footer/Footer'
import Subscribe from './components/subscribe/Subscribe'

export default {
  components: {
    Subscribe,
    Footer,
    News,
    About,
    Header,
    Slider
  }
}
</script>
