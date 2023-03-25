<script>

export default {
    data() {
        return {
            socialLinks: [
                {
                    tag: "F",
                    link: "#"
                },
                {
                    tag: "T",
                    link: "#"
                },
                {
                    tag: "YT",
                    link: "#"
                },
                {
                    tag: "P",
                    link: "#"
                },
                {
                    tag: "G",
                    link: "#"
                },
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
                        <li v-for="link in socialLinks"><a href="link.link">{{ link.tag }}</a></li>
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
            h3{
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