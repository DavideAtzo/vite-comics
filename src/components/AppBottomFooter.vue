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
                    <button>sign-up now!</button>
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
    background-color: #303030;
    

    .container {
        max-width: 1280px;
        margin: 0 auto;

        #joinDC {
            height: 110px;
            display: flex;
            justify-content: space-between;
            align-items: center;

            #socialLinks {
                display: flex;
            }
            button{
                padding: .625rem .9375rem;
                text-transform: uppercase;
                background-color: inherit;
                border: 2px solid #0282f9;
                color: white;
            }
            h3 {
                text-transform: uppercase;
                padding: .3125rem .625rem;
            }

            ul {
                display: flex;
                justify-content: center;
            }

            li {
                padding: 0 10px;
            }
            img{
                width: 35px;
                
            }

        }
    }
}
</style>