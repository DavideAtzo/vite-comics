<script>
    import AppCardElement from './AppCardElement.vue';
    export default {
        components: {
            AppCardElement
        },
        data(){
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
    <section>
        <AppCardElement v-for="content in content" :url="content.thumb" :title="content.series"/>
    </section>
</template>

<style lang="scss" scoped>

</style>