<script>
import AppHeader from "./components/AppHeader.vue";
import AppMainContent from "./components/AppMainContent.vue";
// import AppTopFooter from "./components/AppTopFooter.vue";
// import AppMainFooter from "./components/AppMainFooter.vue";
import AppFooter from './components/AppFooter.vue';
  export default {
    components: {
      AppHeader,
      AppMainContent,
      // AppTopFooter,
      // AppMainFooter
      AppFooter,
    }
  }
</script>

<template>
  <AppHeader></AppHeader>
  <AppMainContent></AppMainContent>
  <AppFooter></AppFooter>
  <!-- <AppTopFooter></AppTopFooter>
  <AppMainFooter></AppMainFooter> -->
</template>

<style lang="scss" scoped>

</style>
