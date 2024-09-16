<script>
export default {
  data() {
    return {
      name: 'AppFooter',
      footerSections: [
        {
          title: 'DC COMICS', 
          items: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News']
        },
        {
          title: 'SHOP',
          items: ['Shop DC', 'Shop DC Collectibles']
        },
        {
          title: 'DC',
          items: ['Terms Of Use', 'Privacy policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
        },
        {
          title: 'SITES',
          items: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
        }
      ]
    }
  }
}
</script>

<template>
  <footer>
    <div class="top-footer">
      <div class="d-flex container">
        <div class="col-md-8 footer-lists">
          <div class="row">
            <div v-for="(section, index) in footerSections" :key="index" class="col">
              <h4>{{ section.title }}</h4>
              <ul>
                <li v-for="(item, idx) in section.items" :key="idx">{{ item }}</li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-md-4 footer-image text-end">
          <img src="../assets/img/dc-logo-bg.png" alt="DC Image">
        </div>
      </div>
    </div>
    <div class="bottom-footer container d-flex justify-content-between">
      <div class="sign-up text-center my-3">
        <button id="join-us" class="btn text-white">SIGN-UP NOW!</button>
      </div>

      <div class="social-media d-flex align-items-center gap-4">
        <p class="mb-0">FOLLOW US</p>
        <div class="social-icons d-flex justify-content-center gap-3">
          <img src="../assets/img/footer-facebook.png" alt="Facebook">
          <img src="../assets/img/footer-twitter.png" alt="Twitter">
          <img src="../assets/img/footer-youtube.png" alt="Youtube">
          <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
          <img src="../assets/img/footer-periscope.png" alt="Periscope">
        </div>
      </div>
    </div>
  </footer>
</template>
  
  <style scoped lang="scss">
    @use '../../style/variables';
    footer {
        background-color: variables.$footer-background-color;
        color: variables.$secondary-color;
    }

  .bottom-footer {
    color: variables.$primary-color;
  }
  
  .top-footer {
    padding: 20px;
    background-image: url(../assets/img/footer-bg.jpg);
  }
  
  .footer-lists {
    h4 {
      margin-bottom: 10px;
    }
    ul {
      list-style: none;
      padding: 0;
      margin-bottom: 20px;
    }
    li {
      margin-bottom: 5px;
      color: variables.$secondary-color;
      cursor: pointer;
    }
  }
  
  .footer-image img {
    width: 80%;
    overflow: hidden;
  }
  
  .social-icons {
    cursor: pointer;
  }

  #join-us {
    border-color: variables.$primary-color;
  }
  </style>
  