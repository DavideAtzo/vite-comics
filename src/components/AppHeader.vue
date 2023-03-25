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
                    <li v-for="link in navLinks"><a href="link.link">{{ link.tag.toUpperCase() }}</a></li>
                </ul>
            </div>
        </div>
    </header>
</template>
<style lang="scss" scoped>
header{
    padding: 20px;
    .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1280px;
    margin: 0 auto;

    ul {
        display: flex;
        justify-content: center;
    }

    a {
        color: black;
    }

    li {
        padding: 10px;
    }
}
}
</style>