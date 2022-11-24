<template>
  <main>
    <div class="main-top">
      <div class="container">
        <h1> -->Content Goes Here  </h1>
      </div>
    </div>
    <div class="main-bot">
      <div class="container">
        <ul>
          <li>
            <a href="!#"><img src="@/img/buy-comics-digital-comics.png" alt="">digital comics</a>
          </li>
          <li>
            <a href="!#"><img src="@/img/buy-comics-merchandise.png" alt="">dc merchandise</a>
          </li>
          <li>
            <a href="!#"><img src="@/img/buy-comics-subscriptions.png" alt="">subscription</a>
          </li>
          <li>
            <a href="!#"><img src="@/img/buy-comics-shop-locator.png" alt="">comic shop locator</a>
          </li>
          <li>
            <a href="!#"><img src="@/img/buy-dc-power-visa.svg" alt="">dc power visa</a>
          </li>
        </ul>
      </div>
    </div>

  </main>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>

.container {
  display: flex;
  align-items: center;
  width: 1200px;
  height: 100%;
  margin: auto;
}

.main-top {
  background-color: #1C1C1C;
  color: white;
  padding: 3rem 0;
}

.main-bot {
  background-color: #0282F9;
  color: white;
  text-transform: uppercase;
  padding: 3rem;
}

.main-bot img {
  height: 40px;
  margin-right: .5rem;
}

.main-bot ul {
  display: flex;
  justify-content: space-around;
  width: 100%;
}

.main-bot li {
  display: flex;
  align-items: center;
}

.main-bot a:hover {
  transition: all .5s linear;
  transform: scale(1.2);
}
</style>
