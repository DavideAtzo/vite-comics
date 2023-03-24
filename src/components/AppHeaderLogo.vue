<script>
export default {
    data() {
        return {
            navLinks: [
                {
                    tag: "characters",
                    link: "#"
                },
                {
                    tag: "comics",
                    link: "#"
                },
                {
                    tag: "movies",
                    link: "#"
                },
                {
                    tag: "tv",
                    link: "#"
                },
                {
                    tag: "games",
                    link: "#"
                },
                {
                    tag: "collectibles",
                    link: "#"
                },
                {
                    tag: "videos",
                    link: "#"
                },
                {
                    tag: "fans",
                    link: "#"
                },
                {
                    tag: "news",
                    link: "#"
                },
                {
                    tag: "shop",
                    link: "#"
                }
            ]
        }
    }
}
</script>
<template>
    <header>
        <div class="container">
            <div id="logoHeader">
                <img src="../assets/img/dc-logo.png" alt="logo-DC">
            </div>
            <div id="navLinks">
                <ul>
                    <li v-for="link in navLinks"><a href="link.link">{{ link.tag }}</a></li>
                </ul>
            </div>
        </div>
    </header>
</template>
<style lang="scss" scoped></style>