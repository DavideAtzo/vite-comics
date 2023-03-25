<script>
import AppCardElement from './AppCardElement.vue';
export default {
    components: {
        AppCardElement
    },
    data() {
        return {
            content: [
                {
                    "thumb": "https://static.dc.com/2023-03/LEGIONOB_Cv1_00111_DIGITAL.jpg?w=640",
                    "series": "DC'S LEGION OF BLOOM",
                },
                {
                    "thumb": "https://static.dc.com/2023-03/FLS_Cv795_79511_DIGITAL.jpg?w=640",
                    "series": "THE FLASH",
                },
                {
                    "thumb": "https://static.dc.com/2023-03/NTW_Cv102_10211_DIGITAL-1.jpg?w=640",
                    "series": "NIGHTWING",
                },
                {
                    "thumb": "https://static.dc.com/2023-03/BMSMWF_Cv13_01311_DIGITAL.jpg?w=640",
                    "series": "BATMAN/SUPERMAN: WORLD'S FINEST",
                },
                {
                    "thumb": "https://static.dc.com/2023-03/CTW_Cv53_05311_DIGITAL.jpg?w=640",
                    "series": "CATWOMAN",
                },
                {
                    "thumb": "https://static.dc.com/2023-03/BA_Cv9_00911_DIGITAL.jpg?w=640",
                    "series": "BLACK ADAM",
                },
                {
                    "thumb": "https://static.dc.com/2023-03/SM_LOST_Cv1_00111_DIGITAL.jpg?w=640",
                    "series": "SUPERMAN: LOST",
                },
                {
                    "thumb": "https://static.dc.com/2023-03/SUPES_Cv2_00211_DIGITAL.jpg?w=640",
                    "series": "SUPERMAN",
                },
                {
                    "thumb": "https://static.dc.com/2023-03/ROBIN_v3%20%28Cover%29.jpg?w=640",
                    "series": "ROBIN VOL. 3: SECRETS AND SHADOWS ",
                },
                {
                    "thumb": "https://static.dc.com/2023-03/HQv3%20%28%20Cover%29.jpg?w=640",
                    "series": "HARLEY QUINN VOL. 3: VERDICT",
                },
                {
                    "thumb": "https://static.dc.com/2023-03/MULTVTJ%20%28COVER%29.jpg?w=640",
                    "series": "MULTIVERSITY: TEEN JUSTICE",
                },
                {
                    "thumb": "https://static.dc.com/2023-03/WW_Cv797_79711_DIGITAL.jpg?w=640",
                    "series": "WONDER WOMAN",
                }
            ]
        }
    }
}
</script>
<template>
    <section id="cardsDC">
        <button id="currentSiries"><a href="#">current siries</a></button>
        <div class="container">
            <AppCardElement v-for="content in content" :url="content.thumb" :title="content.series" />
            <button id="loadMore"><a href="#">load more</a></button>
        </div>

    </section>
</template>

<style lang="scss" scoped>
#cardsDC {

    background-color: #1c1c1c;
    padding: 3.125rem;
    color: white;
    position: relative;

    #currentSiries {
        padding: .625rem .9375rem;
        text-transform: uppercase;
        background-color: #0282f9;
        border: 1px solid #0282f9;
        color: white;
        font-weight: 600;
        position: absolute;
        top: -20px;
        left: 150px;
        cursor: pointer;
    }

    .container {
        max-width: 1280px;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        flex-wrap: wrap;

        div {
            width: calc(100% / 6);
            padding: 1.875rem;

            :deep(img) {
                display: block;
                width: 100%;
                margin-bottom: 1.875rem;
            }
        }
    }

    #loadMore {
        padding: .625rem 3.75rem;
        text-transform: uppercase;
        background-color: #0282f9;
        border: 1px solid #0282f9;
        color: white;
        font-weight: 600;
        cursor: pointer;
    }

}
</style>