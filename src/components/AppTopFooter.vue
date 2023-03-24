<script>
export default {
    data() {
        return {
            topFooterList: [
                {
                    text: "digital comics",
                    img: "src/assets/img/buy-comics-digital-comics.png"
                },
                {
                    text: "dc merchandise",
                    img: "src/assets/img/buy-comics-merchandise.png"
                },
                {
                    text: "subscription",
                    img: "src/assets/img/buy-comics-subscriptions.png"
                },
                {
                    text: "comic shop locator",
                    img: "src/assets/img/buy-comics-shop-locator.png"
                },
                {
                    text: "dc power visa",
                    img: "src/assets/img/buy-dc-power-visa.svg"
                }
            ]
        }
    }
}
</script>

<template>
    <div id="topFooter">
        <div class="container">
            <ul>
                <li v-for="item in topFooterList">
                    <a href="#">
                        <div class="img">
                            <img :src="item.img" alt="">
                        </div>
                        <div class="textImg">
                            {{ item.text.toUpperCase() }}
                        </div>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
#topFooter {
    background-color: #0282f9;

    .container {
        max-width: 1280px;
        margin: 0 auto;

        ul {
            display: flex;
            justify-content: space-around;
            align-items: center;

            a {
                display: flex;
                align-items: center;
                color: white;
                padding: .9375rem;

                img {
                    width: 3.125rem;

                }
                .textImg{
                    padding: .9375rem;
                }
            }

        }
    }
}
</style>