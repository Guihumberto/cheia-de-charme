<template>
    <v-row id="about">
        <sectionTitle :info="contact" />
        <v-col cols="12">
            <v-card>
            <v-card-title>
                CHEIA DE CHARME
            </v-card-title>
            <v-card-text>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad excepturi labore, explicabo inventore fugiat, modi at libero magnam aut in dolor perferendis? Animi, quas soluta aspernatur nostrum rerum nemo voluptate.
            </v-card-text>
            </v-card>
        </v-col>
    </v-row>  
</template>

<script>
export default {
    data(){
      return{
        contact:{
          title: "QUEM SOMOS NÓS",
          subtitle: "Nossa história",
          icon: 'mdi-information-outline'
        }
      }
    }
}
</script>