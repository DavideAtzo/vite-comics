<script>
import AppTopFooter from './AppTopFooter.vue';
import AppMainFooter from './AppMainFooter.vue';
export default {
    components: {
        AppTopFooter,
        AppMainFooter,
    },
    data() {
        return {
        }
    }
}
</script>

<template>
    <footer>
        <AppTopFooter></AppTopFooter>
        <AppMainFooter></AppMainFooter>
    </footer>
</template>

<style lang="scss" scoped></style>