<script>
import AppTopFooter from './AppTopFooter.vue';
import AppMainFooter from './AppMainFooter.vue';
import AppBottomFooter from './AppBottomFooter.vue';
export default {
    components: {
        AppTopFooter,
        AppMainFooter,
        AppBottomFooter
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
        <AppBottomFooter></AppBottomFooter>
    </footer>
</template>

<style lang="scss">
footer{
    background-image: url('../assets/img/dc-logo-bg.png'), url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: auto, cover;
    background-position: 80%, 0%;
}
</style>