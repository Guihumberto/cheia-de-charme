<template>
    <v-row id="header">
    <v-col cols="12" sm="6">
      <v-img src="1.png" contain max-height="500"></v-img>
    </v-col>
    <v-col cols="12" sm="6">
      <v-row>
        <v-col cols="12">
          <v-img max-width="350" src="logo2.jpeg"></v-img>
        </v-col> 
        <v-col cols="12">
          <h5 class="red--text text--darken-4 top">Moda Feminina</h5>
          <h1 class="white--text">Cheia de Charme</h1>
          <p class="grey--text" style="text-align: justify;">
            Nossa loja é especializada em moda feminina e infantil
            em atividade há mais de 10 anos!!
            <br />
            Venha nos fazer uma visita!
          </p>
          <v-btn href="#about" tile color="#A7121D" dark>Sobre </v-btn>
          <v-btn @click="whatsapp" color="success" dark> Contato<v-icon class="ml-1">mdi-whatsapp</v-icon> </v-btn>
          <v-btn icon @click="share" dark > <v-icon>mdi-share-variant</v-icon> </v-btn>
          
        </v-col>
      </v-row>
    </v-col>
    </v-row>
</template>

<script>
  export default {
    methods: {
            share() {
                const urlApi = /Android|webOS|iPhone|iPad|iPod|BlackBerry|BB|PlayBook|IEMobile|Windows Phone|Kindle|Silk|Opera Mini/i.test(navigator.userAgent) ? "https://api.whatsapp.com/send" : "https://web.whatsapp.com/send" 
                const texto = "?text=https://instagram.com/cheiadecharme_loja?igshid=YmMyMTA2M2Y="
                window.open(urlApi + texto, "_blank")
            },
            whatsapp() {
                const urlApi = /Android|webOS|iPhone|iPad|iPod|BlackBerry|BB|PlayBook|IEMobile|Windows Phone|Kindle|Silk|Opera Mini/i.test(navigator.userAgent) ? "https://api.whatsapp.com/send" : "https://web.whatsapp.com/send" 
                const texto = "Olá, gostaria de uma informação."
                window.open(urlApi + "?phone=5598988442459&text=" + texto, "_blank")
            }
    }
  }
</script>
