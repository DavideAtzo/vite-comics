<script>
import AppHeader from "./components/AppHeader.vue";
import AppMainContent from "./components/AppMainContent.vue";
import AppTopFooter from "./components/AppTopFooter.vue";
import AppMainFooter from "./components/AppMainFooter.vue";
  export default {
    components: {
      AppHeader,
      AppMainContent,
      AppTopFooter,
      AppMainFooter
    }
  }
</script>

<template>
  <AppHeader></AppHeader>
  <AppMainContent></AppMainContent>
  <AppTopFooter></AppTopFooter>
  <AppMainFooter></AppMainFooter>
</template>

<style lang="scss" scoped>

</style>
