<template>
  <div id="app">
    <header>
      <Header></Header>
    </header>
    <main>
      <section>
        <Slider></Slider>
      </section>
    </main>
    <footer>

    </footer>

  </div>
</template>

<style lang="scss">
  @import "style/global.scss";
</style>
<script>
import Header from './components/header/Header'
import Slider from './components/slider/Slider'

export default {
  components: { Header, Slider }
}
</script>
