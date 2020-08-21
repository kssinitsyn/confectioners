<template>
  <div class="subscribe__content">
    <form v-if="this.success === false" class="subscribe" action="#" @submit.prevent="checkForm">
      <h2 class="subscribe__title">подпишитесь на рассылку</h2>
      <div class="subscribe__row">
        <div class="subscribe__field">
          <label class="subscribe__label-invalid" v-if="!$v.name.required">Заполните поле</label>
<!--          <label class="subscribe__label-invalid" v-else-if="$v.name.dontAllowNumber">Цифры в имени не допустимы</label>-->
          <label v-else-if="$v.name.required">Имя</label>
          <input class="subscribe__input"
                 id="name"
                 type="text"
                 placeholder="Имя"
                 v-model="name"
                 :class="{invalid: $v.name.dirty && (!$v.name.required) }">
        </div>
        <div class="subscribe__field">
          <label class="subscribe__label-invalid" v-if="!$v.email.required">Заполните поле</label>
          <label class="subscribe__label-invalid" v-else-if="!$v.email.email">Введите корректный Email</label>
          <label v-else-if="$v.email.required">Email</label>
          <input class="subscribe__input"
                 id="email"
                 type="text"
                 placeholder="example@mail.com"
                 v-model="email"
                 :class="{invalid: ($v.name.dirty && (!$v.email.required) || (!$v.email.email)) }">
        </div>
      </div>
      <div class="subscribe__textarea">
        <label class="subscribe__label-invalid" for="comment" v-if="!$v.comment.required">Заполните поле</label>
        <textarea id="comment"
                  cols="30"
                  rows="10"
                  placeholder="Комментарии"
                  v-model="comment"
                  :class="{invalid: $v.comment.dirty && (!$v.comment.required) }">
        </textarea>
      </div>
      <button class="subscribe__submit" type="submit">подписаться</button>
    </form>
    <div v-if="this.success === true" class="subscribe">
      <svg class="subscribe__done" xmlns="http://www.w3.org/2000/svg" width="61" height="61" viewBox="0 0 61 61">
        <defs>
        </defs>
        <g transform="translate(15.555 19.307)">
          <path class="a" d="M135.182,135.04l-14.762,15.036-7.564-7.595-4.056,4.057,11.925,11.9,19.154-18.575Z"
                transform="translate(-108.8 -135.04)"/>
        </g>
        <path class="a"
              d="M30.5,0A30.5,30.5,0,1,0,61,30.5,30.5,30.5,0,0,0,30.5,0Zm0,55.48A24.98,24.98,0,1,1,55.48,30.5,24.98,24.98,0,0,1,30.5,55.48Z"/>
      </svg>
      <p class="subscribe__done-title">Уважаемый, {{this.name}}, спасибо за подписку!</p>
    </div>
  </div>
</template>

<script>
import { email, required } from 'vuelidate/lib/validators'

export default {
  name: 'Subscribe',
  data: function () {
    return {
      name: null,
      email: null,
      comment: null,
      success: false
    }
  },
  validations: {
    name: {
      required
      // dontAllowNumber (name) {
      //   return (
      //     /[^A-Za-z]/.test(name)
      //   )
      // }
    },
    email: {
      required,
      email
    },
    comment: { required }
  },
  methods: {
    checkForm: function (e) {
      if (this.$v.$invalid) {
        this.$v.$touch()
      } else {
        console.log('submit')
        this.success = true
        console.log(this.success)
      }
    }
  }
}
</script>

<style scoped lang="scss">
  @import "subscribe.scss";
</style>
