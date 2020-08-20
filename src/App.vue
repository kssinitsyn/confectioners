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

  .vueperslide__title {
    max-width: 766px;
    margin-bottom: 19px;

    font-family: 'Montserrat', sans-serif;
    font-weight: 600;
    font-size: 46px;
    line-height: 54px;
    color: #FFFFFF;
    text-transform: uppercase;
    text-align: left  ;
  }

  .vueperslide__content {
    max-width: 660px;

    font-family: 'Montserrat', sans-serif;
    font-weight: 400;
    font-size: 24px;
    line-height: 30px;
    color: #FFFFFF;
    text-align: left  ;
  }

  .vueperslide__content-wrapper {
    padding-top: 176px;
    /*max-width: 1170px;*/
    align-items: center !important;
    justify-content: flex-start !important;

    background-color: rgba(0,0,0, 0.56);
  }

  .vueperslides__bullets {
    margin-bottom: 50px;
  }

  .vueperslides__bullet .default {
    background-color: #F7F7F7;
    width: 70px;
    height: 3px;
    border-radius: 0;
    box-shadow: none;
    border: none;
  }

  .vueperslides__bullet--active .default {background-color: #14A5DA;}

  .vueperslides__arrow svg {
    fill: red !important;
  }

  @media screen and (max-width: 1169px) {
    .vueperslide__title {
      max-width: 290px;
      margin-bottom: 19px;

      font-size: 16px;
      line-height: 20px;
    }

    .vueperslide__content {
      max-width: 290px;

      font-size: 14px;
      line-height: 18px;
    }

    .vueperslide__content-wrapper {
      padding-top: 67px !important;
      /*max-width: 290px;*/

      background-color: rgba(0,0,0, 0.56);
    }

    .vueperslides__bullet .default {
      width: 30px;
    }
  }

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
