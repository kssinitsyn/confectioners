<template>
  <nav class="navbar">
    <div class="menu__rules_desktop-wrap">
      <ul class="menu__rules_desktop">
        <li>
          <a class="menu__item" href="">Режим работы</a>
        </li>
        <li>
          <a class="menu__item" href="">Правила посещения</a>
        </li>
      </ul>
    </div>
    <div class="hamburger-menu">
      <a class="logo logo_mobile" href="#">Logotype</a>
      <input id="menu__toggle" type="checkbox" />
      <label class="menu__btn" for="menu__toggle">
        <span></span>
      </label>

      <div class="menu__box">
        <a class="logo" href="#">Logotype</a>
        <ul class="menu__list">
          <li><a class="menu__item" href="#">Меню</a></li>
          <li><a class="menu__item" href="#">Меню</a></li>
          <li><a class="menu__item" href="#">Меню</a></li>
          <li><a class="menu__item" href="#">Меню</a></li>
          <li><a class="menu__item" href="#">Меню</a></li>
          <li><a class="menu__item" href="#">Меню</a></li>
        </ul>
        <ul class="menu__login">
          <li>
            <a class="menu__item" href="">Вход</a>
          </li>
          <li>
            <a class="menu__item" href="">Регистрация</a>
          </li>
        </ul>
        <ul class="menu__rules_mobile">
          <li>
            <a class="menu__item" href="">Режим работы</a>
          </li>
          <li>
            <a class="menu__item" href="">Правила посещения</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style scoped lang="scss">
  @import "header.scss";
</style>
