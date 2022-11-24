<template>
  <div>
    <HeaderSection/>
    <MainSection/>
    <FooterSection/>
  </div>
</template>

<script>
  import HeaderSection from '@/HeaderSection.vue';
  import MainSection from '@/MainSection.vue';
  import FooterSection from '@/FooterSection.vue';
export default {

  components: {
    HeaderSection,
    MainSection,
    FooterSection,
  },
};
</script>

<style>

</style>
