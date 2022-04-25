<template>
  <v-app>
    <navbar />

    <v-main style="background-color: black;">
      <v-container >
        <nuxt />
        <v-btn
          elevation="10"
          color="success"
          fab
          @click="whatsapp"
          id="links-fixos"
        > <v-icon>mdi-whatsapp</v-icon></v-btn>
        <v-dialog v-model="dialog" max-width="500">
          <v-card DARK >
            <v-img src="https://cdn.vuetifyjs.com/images/parallax/material.jpg">
              <v-card-title class="mx-auto px-auto white--text ">Cheia de Charme<v-spacer></v-spacer>
                <v-btn dark @click="dialog= false" icon> <v-icon>mdi-close</v-icon> </v-btn>
              </v-card-title>
              <v-card-title class="display-1 white--text">CUPOM DE DESCONTO</v-card-title>
              <v-card-text>
                <v-img contain max-height="350" src="27.jpeg"></v-img>
              </v-card-text>
              <v-card-actions>
                <v-row justify="center">
                  <v-col cols="12" class=" white--text text-center">
                    Você ganhou 20% de desconto!
                  </v-col>
                  <v-col cols="12" class="my-0 pt-0 text-center" >
                    <v-btn x-large @click="whatsapp" dark color="error" class="mx-auto"> Clique aqui!</v-btn>
                  </v-col>
                </v-row>
              </v-card-actions>
            </v-img>
          </v-card>
        </v-dialog>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
  export default {
    data: () => ({
      dialog: true
    }),
    methods:{
      whatsapp() {
                const urlApi = /Android|webOS|iPhone|iPad|iPod|BlackBerry|BB|PlayBook|IEMobile|Windows Phone|Kindle|Silk|Opera Mini/i.test(navigator.userAgent) ? "https://api.whatsapp.com/send" : "https://web.whatsapp.com/send" 
                const texto = "Olá, gostaria de receber meus 20% de desconto dado pelo site COD: #CHEIADECHARME_LOJA_SITE."
                window.open(urlApi + "?phone=5598988442459&text=" + texto, "_blank")
            },
    }
  }
</script>
<style>
  #links-fixos{
  /*você pode alterar largura usando width*/
  padding:5px;
  background:rgba(0,0,0,0.2);
  position:fixed;
  right: 10px;
  bottom:10px;/*altura da classe*/
}
.tagred{
  border: 4px solid #A7121D;
  margin-right: 4px;
}
</style>