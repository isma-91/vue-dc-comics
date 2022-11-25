<template>
  <div class="card">
    <div class="comic-img">
      <img
        :src="comic.thumb"
        :alt="comic.series"
      >
    </div>
    <h3> {{ comic.series }} </h3>
  </div>
</template>

<script>
export default {
  name: 'DcCard',
  props: {
    comic: Object,
  },
};
</script>

<style lang="scss" scoped>

.card:hover {
  cursor: pointer;
}
.comic-img {
  overflow: hidden;
  img {
  width: 100%;
  margin-bottom: -100px;
  }
}

h3 {
  font-weight: 400;
  text-align: center;
  color: whitesmoke;
  text-transform: uppercase;
  margin-top: .5rem;
}
</style>
