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

<style lang="scss">
footer{
    background-image: url('../assets/img/dc-logo-bg.png'), url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
}
</style>