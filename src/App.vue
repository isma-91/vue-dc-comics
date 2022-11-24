<template>
  <div>
    <HeaderSection/>
    <MainSection/>
    <FooterSection/>
  </div>
</template>

<script>
import HeaderSection from '@/components/HeaderSection.vue';
import MainSection from '@/components/MainSection.vue';
import FooterSection from '@/components/FooterSection.vue';

export default {
  components: {
    HeaderSection,
    MainSection,
    FooterSection,
  },
};
</script>

<style lang="scss">
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

ul {
  list-style: none;
}
</style>
