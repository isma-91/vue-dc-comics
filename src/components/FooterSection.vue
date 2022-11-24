<template>
<footer>
<div class="footer-top">
  <div class="container">
    <div class="left-side">
      <div class="links">
  <h2>DC COMICS</h2>
  <ul>
    <li>Characters</li>
    <li>Comics</li>
    <li>Movies</li>
    <li>TV</li>
    <li>Games</li>
    <li>Videos</li>
    <li>News</li>
  </ul>
  <h2>SHOP</h2>
  <ul>
    <li>Shop DC</li>
    <li>Shop DC Collectibles</li>
  </ul>
      </div>
      <div class="links">
      <h2>DC</h2>
      <ul>
        <li>Terms Of Use</li>
        <li>Privacy policy (New)</li>
        <li>Ad Choices</li>
        <li>Advertising</li>
        <li>Jobs</li>
        <li>Subscriptions</li>
        <li>Talent Workshop</li>
        <li>CPSC Certificates</li>
        <li>Ratings</li>
        <li>Shop Help</li>
        <li>Contact Us</li>
      </ul>
      </div>
      <div class="links">
      <h2>SITES</h2>
      <ul>
        <li>DC</li>
        <li>MAD Magazine</li>
        <li>DC Kids</li>
        <li>DC Universe</li>
        <li>DC Power Visa</li>
      </ul>
      </div>
    </div>
    <div class="right-side">
      <img class="offset" src="@/img/dc-logo-bg.png" alt="">
    </div>
  </div>
</div>
<div class="footer-bot">

</div>
</footer>
</template>

<script>

export default {

};
</script>

<style lang="scss" scoped>

.container {
  display: flex;
  justify-content: space-between;
  width: 1200px;
  height: 100%;
  margin: auto;
}
.footer-top {
  background-image: url('@/img/footer-bg.jpg');
  background-position: center;
  background-size: cover;
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

h2 {
  color: white;
  margin-bottom: 1rem;
}

ul {
  margin-bottom: 2rem;
}

ul li {
  font-size: .8rem;
  line-height: 1.7rem;
  color: #959588;
}

.offset {
  height: 100%;
  margin-bottom: -70px;
  margin-top: -50px;
}
</style>
