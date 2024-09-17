<script>
  export default {
    data() {
      return {
        name: 'AppMain',
      }
    }
  }
</script>

<template>
  <main>
    <div class="content container">
      <p>Content goes here</p>
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