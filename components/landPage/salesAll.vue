<template>
<v-row>
        <v-col
          v-for="(photo, index) in photos"
          :key="index"
          cols="12"
          sm="6"
          md="4"
        >
          <v-card max-height="600">
            <v-img
              :src="photo.src"
              max-width="380"
              height="500"
              
            >
              <span
                class="text-h5 red--text pl-4 pt-4 d-inline-block"
                v-text="photo.text"
              ></span>
            </v-img>

            <v-card-actions class="white justify-center">
              <v-btn
                color="cyan darken-1"
                class="white--text"
                fab
                icon
                small
                @click="whatsapp"
              >
                <v-icon>mdi-whatsapp</v-icon>
              </v-btn>
              <v-btn
                color="red lighten-3"
                class="white--text"
                fab
                icon
                small
                target="_blank"
                href="https://instagram.com/cheiadecharme_loja?igshid=YmMyMTA2M2Y="
              >
                <v-icon>mdi-instagram</v-icon>
              </v-btn>
              <ImgPainel :img="photo" />
            </v-card-actions>
          </v-card>
        </v-col>
</v-row>
</template>

<script>
  export default {
    data: () => ({
      dialog: false,
      photos:[
        {src: '20.jpeg', text: 'Good'},
        {src: '21.jpeg', text: 'Best'},
        {src: '22.jpeg', text: 'Finest'},
        {src: '23.jpeg', text: 'Cheia'},
        {src: '24.jpeg', text: 'de'},
        {src: '25.jpeg', text: 'cheia'},
        {src: '26.jpeg', text: 'de'},
        {src: '27.jpeg', text: 'Charme'},
        {src: '28.jpeg', text: 'Linda'},
        {src: '29.jpeg', text: 'Poderosa'},
        {src: '30.jpeg', text: 'Magnífica'},
        {src: '31.jpeg', text: 'Deslumbrante'},
        {src: '32.jpeg', text: 'Cheia'},
        {src: '33.jpeg', text: 'de'},
        {src: '34.jpeg', text: 'Charme'},
        {src: '35.jpeg', text: 'Magnífica'},
        {src: '36.jpeg', text: 'Deslumbrante'},
        {src: '37.jpeg', text: 'Cheia'},
        {src: '38.jpeg', text: 'de'},
        {src: '39.jpeg', text: 'Charme'},
        {src: '40.jpeg', text: 'Magnífica'},
        {src: '41.jpeg', text: 'Deslumbrante'},
        {src: '42.jpeg', text: 'Cheia'},
        {src: '43.jpeg', text: 'de'},
        {src: '44.jpeg', text: 'Charme'},
        {src: '45.jpeg', text: 'Magnífica'},
        {src: '46.jpeg', text: 'Deslumbrante'},
        {src: '47.jpeg', text: 'Cheia'},
        {src: '48.jpeg', text: 'de'},
        {src: '49.jpeg', text: 'Charme'},
        {src: '50.jpeg', text: 'Magnífica'},
        {src: '51.jpeg', text: 'Deslumbrante'},
      ],
    }),
    methods: {
      getImage () {
        const min = 550
        const max = 560

        return Math.floor(Math.random() * (max - min + 1)) + min
      },
      whatsapp() {
                const urlApi = /Android|webOS|iPhone|iPad|iPod|BlackBerry|BB|PlayBook|IEMobile|Windows Phone|Kindle|Silk|Opera Mini/i.test(navigator.userAgent) ? "https://api.whatsapp.com/send" : "https://web.whatsapp.com/send" 
                const texto = "Olá, gostaria de uma informação."
                window.open(urlApi + "?phone=5598988442459&text=" + texto, "_blank")
            }
    },
  }
</script>