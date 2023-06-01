<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppFooter
  }
}
</script>


<template>
  <header>
    <AppHeader />
  </header>


  <main>
    <div class="text">

    </div>
  </main>

  <footer>
    <AppFooter />
  </footer>
</template>


<style lang="scss">
@use './styles/layout.scss' as*;
</style>
