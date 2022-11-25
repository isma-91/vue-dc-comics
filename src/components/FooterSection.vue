<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <div class="left-side">
          <div class="links">
      <h2>DC COMICS</h2>
      <ul>
        <li><a href="!#">Characters</a></li>
        <li><a href="!#">Comics</a></li>
        <li><a href="!#">Movies</a></li>
        <li><a href="!#">TV</a></li>
        <li><a href="!#">Games</a></li>
        <li><a href="!#">Videos</a></li>
        <li><a href="!#">News</a></li>
      </ul>
      <h2>SHOP</h2>
      <ul>
        <li><a href="!#">Shop DC</a></li>
        <li><a href="!#">Shop DC Collectibles</a></li>
      </ul>
          </div>
          <div class="links">
          <h2>DC</h2>
          <ul>
            <li><a href="!#">Terms Of Use</a></li>
            <li><a href="!#">Privacy policy (New)</a></li>
            <li><a href="!#">Ad Choices</a></li>
            <li><a href="!#">Advertising</a></li>
            <li><a href="!#">Jobs</a></li>
            <li><a href="!#">Subscriptions</a></li>
            <li><a href="!#">Talent Workshop</a></li>
            <li><a href="!#">CPSC Certificates</a></li>
            <li><a href="!#">Ratings</a></li>
            <li><a href="!#">Shop Help</a></li>
            <li><a href="!#">Contact Us</a></li>
          </ul>
          </div>
          <div class="links">
            <h2>SITES</h2>
            <ul>
              <li><a href="!#">DC</a></li>
              <li><a href="!#">MAD Magazine</a></li>
              <li><a href="!#">DC Kids</a></li>
              <li><a href="!#">DC Universe</a></li>
              <li><a href="!#">DC Power Visa</a></li>
            </ul>
          </div>
        </div>
        <div class="right-side">
          <img class="offset" src="@/img/dc-logo-bg.png" alt="">
        </div>
      </div>
    </div>
    <div class="footer-bot">
      <div class="container">
        <div class="cta">
          <button class="btn-cta"> SIGN-UP NOW! </button>
        </div>
        <div class="socials">
          <h2>FOLLOW US</h2>
          <ul>
            <li><img src="@/img/footer-facebook.png" alt=""></li>
            <li><img src="@/img/footer-twitter.png" alt=""></li>
            <li><img src="@/img/footer-youtube.png" alt=""></li>
            <li><img src="@/img/footer-pinterest.png" alt=""></li>
            <li><img src="@/img/footer-periscope.png" alt=""></li>
          </ul>
          <!-- Con le immagini il link non funziona perchè vuole qualcosa scrito dentro -->
        </div>
      </div>
    </div>
  </footer>
</template>

<script>

export default {
  name: 'FooterSection',
};
</script>

<style lang="scss" scoped>
@import '../assets/variables&classes.scss';

.container {
  justify-content: space-between;
}
.footer-top {
  background-image: url('@/img/footer-bg.jpg');
  background-position: center;
  background-size: cover;
  overflow: hidden;
}

.left-side {
display: flex;
gap: 4rem;
}

.right-side {
  display: block;
  height: 100%;
}

.links {
  padding: 2rem 0;
}

.footer-top h2 {
  color: $primary-text-color;
  margin-bottom: 1rem;
}

.footer-top ul {
  margin-bottom: 2rem;
}

.footer-top ul li {
  font-size: .8rem;
  line-height: 1.7rem;
  color: $secondary-text-color;
}

.offset {
  height: 100%;
  margin-bottom: -70px;
  margin-top: -50px;
}

.footer-bot {
  background-color: $dc-primary-background-color;
  padding: 2rem;
}

.footer-bot .btn-cta {
  background-color: $dc-primary-background-color;
  color: $primary-text-color;
  padding: .8rem;
  border: 2px solid $dc-primary-color;
  cursor: pointer;
}

.footer-bot .btn-cta:hover {
  background-color: $dc-primary-color;
}

.socials {
  display: flex;
  align-items: center;
}

.socials h2 {
  color: $dc-primary-color;
}
.socials ul {
  display: flex;
  align-items: center;
}

.socials li {
  margin: 0 1rem;
}

.socials li:hover {
  cursor: pointer;
  filter: brightness(1.8);
  transform: translateY(-10px);
  transition: 0.4s ease-out;
}

footer a:hover {
color: $primary-text-color;
text-decoration: underline;
}
</style>
