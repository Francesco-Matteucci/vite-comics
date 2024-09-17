<script>
  import comicData from '../assets/dc-comics.json';
  import ComicCard from './ComicCard.vue';

  export default {
    components: {
      ComicCard
    },
    data() {
      return {
        name: 'AppMain',
        comics: comicData
      };
    }
  }
</script>

<template>
  <main>
    <div class="content container">
      <div class="row">
        <div class="col-md-2 mb-4" v-for="(comic, index) in comics" :key="index">
          <ComicCard :comic="comic" />
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped lang="scss">
  @use '../../style/_variables.scss' as variables;

  main {
    padding: 20px;
    background-color: variables.$footer-background-color;
    color: variables.$background-color;
    text-align: center;
  }

  .content {
    font-size: 24px;
  }
</style>