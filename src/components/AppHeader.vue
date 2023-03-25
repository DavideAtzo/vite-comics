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
            <nav>
                <div id="logoHeader">
                    <img src="../assets/img/dc-logo.png" alt="logo-DC">
                </div>
                <div id="navLinks">
                    <ul>
                        <li v-for="link in navLinks"><a href="link.link">{{ link.tag.toUpperCase() }}</a></li>
                    </ul>
                </div>
            </nav>
        </div>
    </header>
</template>
<style lang="scss" scoped>
header {
    .container {
        max-width: 1280px;
        margin: 0 auto;
        nav {
            height: 7.5rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            img{
                width: 80px;
            }
            ul {
                display: flex;
                justify-content: center;

            }
            li {
                line-height: 120px;
                padding: 0 10px;
                &:hover {
                    border-bottom: .3125rem solid #0282f9;
                    color: #0282f9;
                }
            }
        }


    }
}</style>