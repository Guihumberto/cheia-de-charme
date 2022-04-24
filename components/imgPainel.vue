<template>
    <v-dialog
      v-model="dialog"
      max-width="800"
      hide-overlay
      transition="dialog-bottom-transition"
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="primary"
          dark
          v-bind="attrs"
          v-on="on"
          text small
        >
        <v-icon>mdi-card-plus</v-icon>
          ampliar
        </v-btn>
      </template>
      <v-card>
          <v-img contain :src="img.src">
              <v-card-title><v-spacer></v-spacer><v-btn @click="dialog=false" color="error" outlined>Fechar<v-icon>mdi-close</v-icon></v-btn></v-card-title>
          </v-img>
      </v-card>
    </v-dialog>
</template>

<script>
export default {
    data(){
        return{
            dialog: false
        }
    },
    props:{
        img:Object
    }
}
</script>
