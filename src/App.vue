<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppHero from './components/AppHero.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppHero,
    AppFooter,
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppHero />
  <AppFooter />
</template>

<style lang="scss">

#app {
  display: flex;
  flex-direction: column;
  height: 100vh;
}

main {
  flex: 1;
}
</style>


<!-- ESERCIZIO FINITO -->