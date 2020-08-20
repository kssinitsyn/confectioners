<template>
  <div class="subscribe__content">
    <form class="subscribe" action="#">
      <h2 class="subscribe__title">подпишитесь на рассылку</h2>
      <div class="subscribe__row">
        <div class="subscribe__field">
          <label for="">Имя</label>
          <input class="subscribe__input" type="text" placeholder="Имя">
        </div>
        <div class="subscribe__field">
          <label for="">Email</label>
          <input class="subscribe__input" type="text" placeholder="example@mail.com">
        </div>
      </div>
      <div class="subscribe__textarea">
        <label for=""></label>
        <textarea name="" id="" cols="30" rows="10" placeholder="Комментарии"></textarea>
      </div>
      <button class="subscribe__submit">подписаться</button>
    </form>
  </div>
</template>

<script>
export default {
  name: 'Subscribe'
}
</script>

<style scoped lang="scss">
  @import "subscribe.scss";
</style>
