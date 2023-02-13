<script>
export default {
  name: 'AppFooter',
  data() {
    return {
        comicLinks: [
            'Characters',
            'Comics',
            'Movies',
            'TV',
            'Games',
            'Videos',
            'News',
        ],
        shopLinks: [
            'Shop DC',
            'Shop DC Collectibles',
        ],
        dcLinks:[
            'Terms of use',
            'Privacy policy (New)',
            'Ad Choices',
            'Advertising',
            'Jobs',
            'Subscriptions',
            'Talent Workshops',
            'CPSC Certificates',
            'Ratings',
            'Shop Help',
            'Contact Us',
        ],
        sitesLinks: [
            'DC',
            'MAD Magazine',
            'DC Kids',
            'DC Universe',
            'DC Power Visa',
        ]
    }
  }
}
</script>

<template>
    <section class="footer-list">
      <div class="container">
        <div>
              <h3>DC COMICS</h3>
              <ul>
              <li v-for="link in comicLinks"><a href="">{{link}}</a></li>
              </ul>
              <h3>SHOP</h3>
              <ul>
              <li v-for="link in shopLinks"><a href="">{{link}}</a></li>
              </ul>
        </div>
        <div>
          <h3>DC</h3>
          <ul>
            <li v-for="link in dcLinks"><a href="">{{link}}</a></li>
          </ul>
        </div>
        <div>
          <h3>SITES</h3>
          <ul>
            <li v-for="link in sitesLinks"><a href="">{{link}}</a></li>
          </ul>
        </div>
      </div>
    </section>
    <section class="footer-social">
    <div class="container">
      <div>
        <button class="btn-footer">SIGN-UP NOW!</button>
      </div>
      <div class="social-circles">
            <h4>FOLLOW US</h4>
            <img src="../assets/img/footer-facebook.png" alt="facebook" />
            <img src="../assets/img/footer-twitter.png" alt="twitter" />
            <img src="../assets/img/footer-youtube.png" alt="youtube" />
            <img src="../assets/img/footer-pinterest.png" alt="pinterest" />
            <img src="../assets/img/footer-periscope.png" alt="periscope" />
        </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&display=swap');

.footer-list { 
    font-family: 'Open Sans', sans-serif;
    height: 450px;
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;  
    .container {
      background-image: url("../assets/img/dc-logo-bg.png");
      height: 100%;
      background-repeat: no-repeat;
      background-position: right;
      display: flex;
      margin-left: 30px;
      h3 {
        color: white;
        margin-top: 50px;
      }
      ul {
        list-style: none;
        margin-top: 20px;
        a {
          text-decoration: none;
          font-size: 13px;
          padding: 15px 25px 0 0;
          color: #787878;
        }
        a:hover {
          color: white;
        }
      }
    }
}
.footer-social {
    font-family: 'Open Sans', sans-serif;
    background-color: #303030;
    padding: 30px;
    .container {
        display: flex;
        justify-content: space-between;
    }
    .btn-footer {
        color: white;
        background-color: #303030;
        padding: 10px;
    }
    .btn-footer:hover {
        border-color: #0282f9;
    }
    .social-circles {
        display: flex;
        align-items: center;
        justify-content: space-around;
        min-width: 400px;
        width: 30%;
        h4{
        color: #0282f9;
        }
    }
}

</style>