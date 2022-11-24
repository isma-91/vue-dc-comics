<template>
<header class="header">
  <nav class="container">
    <div class="logo">
      <img src="@/img/dc-logo.png" alt="">
    </div>
    <ul>
      <li><a href="#">characters</a></li>
      <li><a href="#">comics</a></li>
      <li><a href="#">movies</a></li>
      <li><a href="#">tv</a></li>
      <li><a href="#">games</a></li>
      <li><a href="#">collectibles</a></li>
      <li><a href="#">videos</a></li>
      <li><a href="#">fans</a></li>
      <li><a href="#">news</a></li>
      <li><a href="#">shop</a></li>
    </ul>
  </nav>
</header>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
.header {
  height: 120px;
  display: flex;
  align-items: center;
}

.container {
  display: flex;
  align-items: center;
  width: 1200px;
  height: 100%;
  margin: auto;
}

.logo {
  height: 70%;
}

header img {
  height: 100%;
}

header img:hover {
  cursor: pointer;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

ul {
  display: flex;
  height: 100%;
}

nav li {
  display: flex;
  align-items: center;
  position: relative;
  margin: 0 .7rem;
  text-transform: uppercase;
  font-weight: bold;
  height: 100%;
}

nav li:hover {
  cursor: pointer;
  color: #2f8cd7;
}

nav li:after {
  content: "";
  position: absolute;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 5px;
  background-color: #2f8cd7;
  display: none;
}

nav li:hover:after {
  display: block;
}

</style>
