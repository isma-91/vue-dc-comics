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
@import '../assets/variables&classes.scss';

.card {
  color: whitesmoke;
}
.comic-img {
  overflow: hidden;
  img {
  width: 100%;
  margin-bottom: -90px;
  }
}

h3 {
  font-weight: 400;
  text-align: center;
  text-transform: uppercase;
  margin-top: .5rem;
}
</style>
