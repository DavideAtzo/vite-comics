<script>
export default {
    data() {
        return {
            dcComicsLinks: {
                linksTitle: 'dc comincs',
                links: [
                    "Characters",
                    "Comics",
                    "Movies",
                    "TV",
                    "Games",
                    "Videos",
                    "News"
                ]
            },
            shopLinks: {
                linksTitle: 'shop',
                links: [
                    "Shop DC",
                    "Shop DC Collectibles"
                ]
            },
            dcLinks: {
                linksTitle: 'dc',
                links: [
                    "Terms Of Use",
                    "Privacy Policy (New)",
                    "Ad Choices",
                    "Advertising",
                    "Jobs",
                    "Subscriptions",
                    "Talent Workshops",
                    "CPSC Certificates",
                    "Ratings",
                    "Shop Help",
                    "Contact Us"
                ]
            },
            sitesLinks: {
                linksTitle: 'sites',
                links: [
                    "DC",
                    "MAD Magazine",
                    "DC Kids",
                    "DC Universe",
                    "DC Power Visa"
                ]
            }
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="mainFooter">
            <div>
                <div id="dcComics">
                <h3>{{ dcComicsLinks.linksTitle.toUpperCase() }}</h3>
                <ul>
                    <li v-for="link in dcComicsLinks.links"><a href="">{{ link }}</a></li>
                </ul>
            </div>
            <div id="shop">
                <h3>{{ shopLinks.linksTitle.toUpperCase() }}</h3>
                <ul>
                    <li v-for="link in shopLinks.links"><a href="">{{ link }}</a></li>
                </ul>
            </div>
            </div>
            <div id="dc">
                <h3>{{ dcLinks.linksTitle.toUpperCase() }}</h3>
                <ul>
                    <li v-for="link in dcLinks.links"><a href="">{{ link }}</a></li>
                </ul>
            </div>
            <div id="sities">
                <h3>{{ sitesLinks.linksTitle.toUpperCase() }}</h3>
                <ul>
                    <li v-for="link in sitesLinks.links"><a href="">{{ link }}</a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.container {
    max-width: 1280px;
    margin: 0 auto;

    .mainFooter {
        width: 35%;
        display: flex;
        justify-content: flex-start;
        color: white;
        padding: 30px 0;
        h3{
            margin: .9375rem 0;
        }
        li{
            line-height: 1.5625rem;
        }
        a{
            color: white;
            opacity: 0.4;
        }
        #dc{
            padding: 0 1.25rem;
        }
    }
}
</style>