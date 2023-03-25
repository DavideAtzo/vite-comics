<script>
import AppHeader from "./components/AppHeader.vue";
import AppMainContent from "./components/AppMainContent.vue";
import AppFooter from './components/AppFooter.vue';
  export default {
    components: {
      AppHeader,
      AppMainContent,
      AppFooter,
    }
  }
</script>

<template>
  <AppHeader></AppHeader>
  <AppMainContent></AppMainContent>
  <AppFooter></AppFooter>
</template>

<style lang="scss" scoped>

</style>
