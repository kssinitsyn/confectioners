<template>
  <div class="news__content">
    <div class="news__header">
      <h2 class="news__title">Новости</h2>
      <a href="" class="news__allnews">Все новости</a>
    </div>
    <div class="news__grid">
      <div class="news__img" v-for="item in items" :key="item.id">
        <img class="news__img-src" :src = item.image alt="">
      </div>
    </div>
    <button class="news__more" @click="loadMore()">показать еще</button>
  </div>
</template>

<script>
export default {
  name: 'News',
  data: function () {
    return {
      items: [
        { image: require('@/assets/img_1.jpg'), id: 1 },
        { image: require('@/assets/img_2.jpg'), id: 2 },
        { image: require('@/assets/img_3.jpg'), id: 3 }
      ]
    }
  },
  methods: {
    loadMore: function () {
      this.items.push({ image: require('@/assets/img_1.jpg') })
      this.items.push({ image: require('@/assets/img_2.jpg') })
      this.items.push({ image: require('@/assets/img_3.jpg') })
    }
  },
  mounted () {
    const el = document.querySelectorAll('.news__img')
    el.forEach((item, i) => {
      item.dataset.content = `${i + 1}`
    })
  }
}
</script>

<style scoped lang="scss">
  @import "news.scss";
</style>
