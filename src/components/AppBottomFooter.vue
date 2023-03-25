<script>

export default {
    data() {
        return {
            socialLinks: [
                {
                    img: 'src/assets/img/footer-facebook.png',
                    name: 'logo-facebook',
                },
                {
                    img: 'src/assets/img/footer-twitter.png',
                    name: 'logo-twitter',
                },
                {
                    img: 'src/assets/img/footer-youtube.png',
                    name: 'logo-youtube',
                },
                {
                    img: 'src/assets/img/footer-pinterest.png',
                    name: 'logo-pinterest',
                },
                {
                    img: 'src/assets/img/footer-periscope.png',
                    name: 'logo-periscope',
                }
            ]
        }
    }
}
</script>

<template>
    <div id="bottomFooter">
        <div class="container">
            <div id="joinDC">
                <div class="btnSignUp">
                    <button>sign-up</button>
                </div>
                <div id="socialLinks">
                    <h3>follow us</h3>
                    <ul>
                        <li v-for="link in socialLinks">
                            <a href="#">
                                <img :src="link.img" :alt="link.name">
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>

    </div>
</template>

<style lang="scss">
#bottomFooter {
    background-color: grey;

    .container {
        max-width: 1280px;
        margin: 0 auto;

        #joinDC {
            display: flex;
            justify-content: space-between;
            padding: 1.25rem 0;

            #socialLinks {
                display: flex;
            }

            h3 {
                text-transform: uppercase;
            }

            ul {
                display: flex;
                justify-content: center;
            }

            li {
                padding: 0 10px;
            }

        }
    }
}
</style>