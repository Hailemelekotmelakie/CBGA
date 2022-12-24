<template>
  <UpperHeader></UpperHeader>
  <AppHeader></AppHeader>
  <AppFooter></AppFooter>
  <AppFooterBelow></AppFooterBelow>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';
import UpperHeader from '@/components/UpperHeader.vue';
import AppFooter from '@/components/AppFooter.vue';
import AppFooterBelow from '@/components/AppFooterBelow.vue';

export default {
  name:"#MainApp",
  components: {
    AppHeader: AppHeader,
    AppFooter:AppFooter,
    UpperHeader:UpperHeader,
    AppFooterBelow:AppFooterBelow
  }
}
</script>

<style>

body {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #f0f2ff;
  margin: 0px;
  padding: 0px;
}
</style>
