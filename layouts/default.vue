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
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
  export default {
    data: () => ({
      
    }),
    methods:{
      whatsapp() {
                const urlApi = /Android|webOS|iPhone|iPad|iPod|BlackBerry|BB|PlayBook|IEMobile|Windows Phone|Kindle|Silk|Opera Mini/i.test(navigator.userAgent) ? "https://api.whatsapp.com/send" : "https://web.whatsapp.com/send" 
                const texto = "Olá, gostaria de uma informação."
                window.open(urlApi + "?phone=5598988442459&text=" + texto, "_blank")
            }
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
</style>