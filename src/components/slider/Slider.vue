<template>
  <div ref="mySlider" class="swiper-container">
    <div class="swiper-wrapper">
      <div class="swiper-slide slide">
        <img class="slider__img" src="@/assets/slide_1.jpg" alt="">
        <div class="slider__content">
          <p class="slider__animation">анимация</p>
          <p class="slider__title">Подготовка спрайтов для анимации в Unity</p>
          <p class="slider__subtitle">Спрайты должны немного отличаться друг от друга, чтобы было заметно движение.</p>
        </div>
      </div>
      <div class="swiper-slide slide">
        <img class="slider__img" src="@/assets/slide_2.jpg" alt="">
        <div class="slider__content">
          <p class="slider__animation">анимация</p>
          <p class="slider__title">Подготовка спрайтов для анимации в Unity</p>
          <p class="slider__subtitle">Спрайты должны немного отличаться друг от друга, чтобы было заметно движение.</p>
        </div>
      </div>
      <div class="swiper-slide slide">
        <img class="slider__img" src="@/assets/slide_3.jpg" alt="">
        <div class="slider__content">
          <p class="slider__animation">анимация</p>
          <p class="slider__title">Подготовка спрайтов для анимации в Unity</p>
          <p class="slider__subtitle">Спрайты должны немного отличаться друг от друга, чтобы было заметно движение.</p>
        </div>
      </div>
    </div>
    <div class="swiper-pagination"></div>
    <div @click="prev" class="swiper-button-prev"></div>
    <div @click="next" class="swiper-button-next"></div>
  </div>
</template>

<script>
import Swiper from 'swiper'
import 'swiper/swiper-bundle.css'

export default {
  data () {
    return {
      slider: null,
      mySliderOptions: {
        loop: true
      }
    }
  },
  methods: {
    next () {
      this.slider.slideNext()
    },
    prev () {
      this.slider.slidePrev()
    }
  },
  mounted () {
    this.slider = new Swiper(this.$refs.mySlider, {
      loop: true,

      pagination: {
        el: '.swiper-pagination'
      },

      navigation: {
        nextEl: '.swiper-button-next',
        prevEl: '.swiper-button-prev'
      }
    })
  }
}
</script>

<style scoped lang="scss">
  @import "slider";

  .swiper-container {
    width: 100vw;
    height: 600px;
    margin: 0 auto;
  }
</style>
