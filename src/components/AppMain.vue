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
  main {
    padding: 20px;
    background-color: #333;
    color: #fff;
    text-align: center;
  }
  
  .content {
    font-size: 24px;
  }
</style>