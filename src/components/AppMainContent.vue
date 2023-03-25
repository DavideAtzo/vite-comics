<script>
import AppJumbo from "./AppJumbo.vue";
import AppDcContent from "./AppDcContent.vue";
import AppTagContent from "./AppTagContent.vue";
export default {
    components: {
        AppJumbo,
        AppDcContent,
        AppTagContent
    }
  }
</script>

<template>
    <main>
        <AppJumbo></AppJumbo>
        <AppTagContent></AppTagContent>
        <AppDcContent></AppDcContent>
    </main>
</template>

<style lang="scss" scoped>

</style>