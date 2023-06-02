<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import List from './components/List.vue';

export default {
  components: {
    AppHeader,
    AppFooter,
    List
  }
}
</script>


<template>
  <header>
    <AppHeader />
  </header>


  <main>
    <List />
  </main>

  <footer>
    <AppFooter />
  </footer>
</template>


<style lang="scss">
@use './styles/layout.scss' as*;
</style>
