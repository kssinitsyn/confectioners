<template>
  <vueper-slides :touchable="false">
    <vueper-slide v-for="(slide, i) in slides"
                  :image="slide.image"
                  :key="i"
                  :title="slide.title"
                  :content="slide.content"
                  :animation="slide.animation"/>
    <template v-slot:arrow-left>
      <i class="icon icon-arrow-left"/>
    </template>

    <template v-slot:arrow-right>
      <svg class="icon icon-arrow-left" xmlns="http://www.w3.org/2000/svg" width="31.495" height="22.141" viewBox="0 0 31.495 22.141" fill="red">
        <path class="a"
              d="M10.273,5.009A1.117,1.117,0,0,1,11.86,6.58L3.813,14.627H30.367a1.118,1.118,0,0,1,1.127,1.111,1.131,1.131,0,0,1-1.127,1.127H3.813L11.86,24.9a1.139,1.139,0,0,1,0,1.587,1.112,1.112,0,0,1-1.587,0L.321,16.532a1.12,1.12,0,0,1,0-1.571Z"
              transform="translate(0.001 -4.676)"/>
      </svg>
    </template>
  </vueper-slides>
</template>

<script>
import { VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css'

export default {
  components: {
    VueperSlides,
    VueperSlide
  },
  data: () => ({
    slides: [
      {
        image: require('@/assets/slide_1.jpg'),
        title: 'Подготовка спрайтов для анимации в Unity',
        content: 'Спрайты должны немного отличаться друг от друга, чтобы было заметно движение.',
        animation: 'Animation'
      },
      {
        image: require('@/assets/slide_2.jpg'),
        title: 'Подготовка спрайтов для анимации в Unity',
        content: 'Спрайты должны немного отличаться друг от друга, чтобы было заметно движение.'
      },
      {
        image: require('@/assets/slide_3.jpg'),
        title: 'Подготовка спрайтов для анимации в Unity',
        content: 'Спрайты должны немного отличаться друг от друга, чтобы было заметно движение.'
      }
    ]
  })
}
</script>

<style scoped lang="scss">
  @import "slider";
</style>
