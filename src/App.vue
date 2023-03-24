<script>
import AppHeader from "./components/AppHeader.vue";
import AppMainContent from "./components/AppMainContent.vue";
import AppTopFooter from "./components/AppTopFooter.vue";
  export default {
    components: {
      AppHeader,
      AppMainContent,
      AppTopFooter
    }
  }
</script>

<template>
  <AppHeader></AppHeader>
  <AppMainContent></AppMainContent>
  <AppTopFooter></AppTopFooter>
</template>

<style lang="scss" scoped>

</style>
