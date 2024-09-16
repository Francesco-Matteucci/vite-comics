<script>
export default {
  data() {
    return {
      name: 'AppFooter',
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
              <div class="col">
                <h4>DC COMICS</h4>
                <ul>
                  <li>Characters</li>
                  <li>Comics</li>
                  <li>Movies</li>
                  <li>TV</li>
                  <li>Games</li>
                  <li>Videos</li>
                  <li>News</li>
                </ul>
                <h4>SHOP</h4>
                <ul>
                  <li>Shop DC</li>
                  <li>Shop DC Collectibles</li>
                </ul>
              </div>
              <div class="col">
                <h4>DC</h4>
                <ul>
                  <li>Terms Of Use</li>
                  <li>Privacy policy (New)</li>
                  <li>Ad Choices</li>
                  <li>Advertising</li>
                  <li>Jobs</li>
                  <li>Subscriptions</li>
                  <li>Talent Workshops</li>
                  <li>CPSC Certificates</li>
                  <li>Ratings</li>
                  <li>Shop Help</li>
                  <li>Contact Us</li>
                </ul>
              </div>
              <div class="col">
                <h4>SITES</h4>
                <ul>
                  <li>DC</li>
                  <li>MAD Magazine</li>
                  <li>DC Kids</li>
                  <li>DC Universe</li>
                  <li>DC Power Visa</li>
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
          <button class="btn btn-primary">SIGN-UP NOW!</button>
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
  footer {
    background-color: #222;
    color: #fff;
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
      color: #7D8181;
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
  </style>
  