<script>
export default {
  data() {
    return {
      name: 'AppHeader',
      navItems: [
        { name: 'Characters', active: false },
        { name: 'Comics', active: true },
        { name: 'Movies', active: false },
        { name: 'TV', active: false },
        { name: 'Games', active: false },
        { name: 'Collectibles', active: false },
        { name: 'Videos', active: false },
        { name: 'Fans', active: false },
        { name: 'News', active: false },
        { name: 'Shop', active: false }
      ]
    }
  },
  methods: {
    setActive(index) {
      this.navItems.forEach((item, i) => {
        // Imposto l'item attivo in base all'indice
        item.active = i === index;
      });
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
            <li v-for="(item, index) in navItems" :key="index"  :class="{ active: item.active }" @click="setActive(index)">
            {{ item.name }}
            </li>
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
li.active {
    color: #007bff;
}
  </style>