<template>
    <v-container fluid style="max-width: 1080px" id="contact">
        <v-row id="store">
            <sectionTitle :info="sectionBar" id="sales" />
            <landPage-salesAll id="about" />
        </v-row>
    </v-container>
</template>

<script>
    export default {
        data(){
            return{
                sectionBar:{
                    title: "Tendências",
                    subtitle: "Lançamentos na Cheia de Charme",
                    btn: true,
                    btnTitle: 'Voltar',
                    url: '/'
                }
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>