<script>
  export default {
    name: 'AppHero',
    data() {
      return {
        icons: [
          { name: 'Digital Comics', img: '../src/assets/img/buy-comics-digital-comics.png' },
          { name: 'DC Merchandise', img: '../src/assets/img/buy-comics-merchandise.png' },
          { name: 'Subscription', img: '../src/assets/img/buy-comics-subscriptions.png' },
          { name: 'Comic Shop Locator', img: '../src/assets/img/buy-comics-shop-locator.png' },
          { name: 'DC Power Visa', img: '../src/assets/img/buy-dc-power-visa.svg' }
        ]
      }
    }
  }
</script>

<template>
  <section class="hero">
    <div class="bg-hero d-flex align-items-center container">
      <div v-for="(icon, index) in icons" :key="index" class="hero-icon">
        <img :src="icon.img" :alt="icon.name"> {{ icon.name }}
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  @use '../../style/_variables.scss' as variables;

  .hero {
    color: variables.$title-color;
    background-color: variables.$background-hero-color;
    padding: 20px 0;
    height: 200px;
    position: relative;
    z-index: 3;
  }

  .bg-hero {
    height: 100%;
  }

  .hero-icon {
    margin: 0 auto;

    img {
      height: 50px;
      cursor: pointer;
      margin-right: 20px;
    }

    &:last-child img {
      height: 35px;
    }
  }
</style>