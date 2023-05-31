<script>
import AppHeader from './components/AppHeader.vue'

export default {
  components: {
    AppHeader
  }
}
</script>


<template>
  <header>
    <div class="container">

      <AppHeader />
    </div>
  </header>

  <main>
    <div class="text">
      <div class="container"></div>
    </div>
    <div class="jumbotron">
      <div class="container"></div>
    </div>
    <div class="site-map">
      <div class="container"></div>
    </div>
  </main>

  <footer>
    <div class="container"></div>
  </footer>
</template>


<style lang="scss">
@use './styles/layout.scss' as*;
</style>
