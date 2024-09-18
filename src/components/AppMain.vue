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
    <div class="jumbotron mb-4"></div>
    <div id="dc-main" class="content container">
      <div class="row">
        <div class="col-md-2 mb-4" v-for="(comic, index) in comics" :key="index">
          <ComicCard :comic="comic" />
        </div>
      </div>

    </div>
    <button class="btn cd-btn">LOAD MORE</button>
  </main>
</template>

<style scoped lang="scss">
  @use '../../style/_variables.scss' as variables;

  main {
    padding-bottom: 20px;
    background-color: variables.$footer-background-color;
    color: variables.$background-color;
    text-align: center;

    button {

      border-color: variables.$primary-color;
      color: variables.$title-color;
      transition: background-color 0.3s ease, transform 0.3s ease;

      &:hover {
        background-color: variables.$background-color;
        color: variables.$primary-color;
        transform: scale(1.05);
        box-shadow: 0px 4px 15px rgba(0, 123, 255, 0.6);
      }
    }
  }


  .content {
    font-size: 24px;
  }

  .jumbotron {
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    height: 200px;
  }

  #dc-main {
    position: relative;
    box-shadow: 30px 30px 70px #000;
    margin-bottom: 30px;
  }

</style>