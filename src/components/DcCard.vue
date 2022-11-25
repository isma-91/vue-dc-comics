<template>
  <div class="card">
    <img
      :src="comic.thumb"
      :alt="comic.series"
    >
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

</style>
