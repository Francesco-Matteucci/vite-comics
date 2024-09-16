<script>
export default {
  data() {
    return {
      name: 'AppHeader',
    }
  }
}
</script>

<template>
    <header>
      <div class="d-flex justify-content-center align-items-center container">
        <div class="col-2 logo">
          <img src="../assets/img/dc-logo.png" alt="Logo DC">
        </div>
        <nav class="col-10">
          <ul class="nav-menu list-inline d-flex justify-content-end gap-3">
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Collectibles</li>
            <li>Videos</li>
            <li>Fans</li>
            <li>News</li>
            <li>Shop</li>
          </ul>
        </nav>
      </div>
    </header>
  </template>
  
  <style scoped lang="scss">
  header {
    padding: 10px 0;
    background-color: #fff;
  }
  
  .logo img {
    height: 80px;
  }
  
  .nav-menu li {
    cursor: pointer;
    font-weight: bold;
    color: #000;
  }
  </style>