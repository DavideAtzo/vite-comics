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
        <div id="dcComics">
            <h2>{{ dcComicsLinks.linksTitle }}</h2>
            <ul>
                <li v-for="link in dcComicsLinks.links"><a href="">{{ link }}</a></li>
            </ul>
        </div>
        <div id="shop">
            <h2>{{ shopLinks.linksTitle }}</h2>
            <ul>
                <li v-for="link in shopLinks.links"><a href="">{{ link }}</a></li>
            </ul>
        </div>
        <div id="dc">
            <h2>{{ dcLinks.linksTitle }}</h2>
            <ul>
                <li v-for="link in dcLinks.links"><a href="">{{ link }}</a></li>
            </ul>
        </div>
        <div id="sities">
            <h2>{{ sitesLinks.linksTitle }}</h2>
            <ul>
                <li v-for="link in sitesLinks.links"><a href="">{{ link }}</a></li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped></style>