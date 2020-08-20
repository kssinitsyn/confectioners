<template>
  <footer class="footer">
    <div class="footer__content">
      <a class="footer__logo" href="#">Logotype</a>
      <div class="footer__grid">
        <div class="footer__left-column">
          <p class="footer__address">г. Москва, метро Бауманская, ул. Бауманская, дом 44</p>
          <a class="footer__tel" href="tel:+70000000000">+7 000 000 00 00</a>
        </div>
        <div class="footer__right-column">
          <ul class="footer__list">
            <li class="footer__item">
              <a href="#" class="footer__link">О компании</a>
            </li>
            <li class="footer__item">
              <a href="#" class="footer__link">Партнёрская программа</a>
            </li>
            <li class="footer__item">
              <a href="#" class="footer__link">Реклама</a>
            </li>
            <li class="footer__item">
              <a href="#" class="footer__link">Пресс-центр</a>
            </li>
            <li class="footer__item">
              <a href="#" class="footer__link">Вакансии</a>
            </li>
            <li class="footer__item">
              <a href="#" class="footer__link">Помощь</a>
            </li>
            <li class="footer__item">
              <a href="#" class="footer__link">Правила</a>
            </li>
          </ul>
          <div class="footer__column-inner">
            <div class="footer__social">
              <p class="footer__social-title">Мы в соц. сетях</p>
              <div class="footer__social-icons">
                <a class="footer__social-icon" href="#">
                  <svg xmlns="http://www.w3.org/2000/svg" width="6.658" height="14.267" viewBox="0 0 6.658 14.267">
                    <g transform="translate(-114.696 -0.001)">
                      <path class="a"
                            d="M116.135,2.764V4.728H114.7v2.4h1.439v7.138h2.956V7.13h1.984s.186-1.152.276-2.411H119.1V3.077a.7.7,0,0,1,.641-.576h1.611V0h-2.19C116.062,0,116.135,2.405,116.135,2.764Z"
                            transform="translate(0 0)"/>
                    </g>
                  </svg>
                </a>
                <a class="footer__social-icon" href="#">
                  <svg xmlns="http://www.w3.org/2000/svg" width="10.913" height="15.6" viewBox="0 0 10.913 15.6">
                    <g transform="translate(-76.922)">
                      <g transform="translate(78.478)">
                        <g transform="translate(0)">
                          <path class="a"
                                d="M131.9,0a3.9,3.9,0,1,0,3.9,3.9A3.9,3.9,0,0,0,131.9,0Zm0,5.85a1.95,1.95,0,1,1,1.95-1.95A1.952,1.952,0,0,1,131.9,5.85Z"
                                transform="translate(-128.002)"/>
                        </g>
                      </g>
                      <g transform="translate(76.922 7.406)">
                        <g transform="translate(0)">
                          <path class="a"
                                d="M87.55,243.35a.974.974,0,0,0-1.379,0,5.37,5.37,0,0,1-7.584,0,.975.975,0,1,0-1.379,1.38,7.268,7.268,0,0,0,4.336,2.085l-2.78,2.78a.975.975,0,1,0,1.379,1.379l2.236-2.236,2.236,2.236a.975.975,0,1,0,1.379-1.379l-2.78-2.78a7.268,7.268,0,0,0,4.336-2.085A.976.976,0,0,0,87.55,243.35Z"
                                transform="translate(-76.922 -243.064)"/>
                        </g>
                      </g>
                    </g>
                  </svg>
                </a>
                <a class="footer__social-icon" href="#">
                  <svg xmlns="http://www.w3.org/2000/svg" width="15.462" height="15.462" viewBox="0 0 15.462 15.462">
                    <path class="a"
                          d="M11.195,0H4.267A4.272,4.272,0,0,0,0,4.267v6.928a4.272,4.272,0,0,0,4.267,4.267h6.928a4.272,4.272,0,0,0,4.267-4.267V4.267A4.272,4.272,0,0,0,11.195,0Zm2.9,11.195a2.9,2.9,0,0,1-2.9,2.9H4.267a2.9,2.9,0,0,1-2.895-2.9V4.267a2.9,2.9,0,0,1,2.895-2.9h6.928a2.9,2.9,0,0,1,2.9,2.9v6.928Z"/>
                    <path class="a"
                          d="M44.952,40.97a3.984,3.984,0,1,0,3.984,3.984A3.989,3.989,0,0,0,44.952,40.97Zm0,6.6a2.612,2.612,0,1,1,2.612-2.612A2.615,2.615,0,0,1,44.952,47.566Z"
                          transform="translate(-37.221 -37.223)"/>
                    <path class="a" d="M119.927,28.251a1.005,1.005,0,1,0,.712.294A1.01,1.01,0,0,0,119.927,28.251Z"
                          transform="translate(-108.045 -25.667)"/>
                  </svg>
                </a>
              </div>
            </div>
            <div class="footer__subscribe">
              <p class="footer__subscribe-title">Подписка на новости</p>
              <form action="#">
                <input class="footer__input" type="text" placeholder="example@mail.com" required>
                <button class="footer__submit">Ok</button>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="footer__bottom">
      <div class="footer__bottom-content">
        <p class="footer__bottom-text">
          © ООО «Глобус», 2016 — 2019
        </p>
        <div class="footer__policy">
          <a class="footer__bottom-link" href="#">
            Политика конфиденциальности
          </a>
          <a class="footer__bottom-link" href="#">Cookies</a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped lang="scss">
  @import "footer.scss";
</style>
