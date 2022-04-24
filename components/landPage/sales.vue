<template>
    <v-row id="sales">
        <sectionTitle :info="contact" />
        <v-col
          v-for="(photo, index) in photos"
          :key="index"
          cols="12"
          sm="6"
          md="4"
        >
          <v-card @click="dialog = true">
            <v-img
              :src="photo.src"
              height="300px"
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
            </v-card-actions>
          </v-card>
          <v-dialog v-model="dialog">
           
          </v-dialog>
        </v-col>
      </v-row>
</template>

<script>
  export default {
    data: () => ({
      dialog: false,
      photos:[
        {src: '2.jpeg', text: 'Good'},
        {src: '3.jpeg', text: 'Best'},
        {src: '4.jpeg', text: 'Finest'},
        {src: '5.jpeg', text: 'Cheia'},
        {src: '6.jpeg', text: 'de'},
        {src: '7.jpeg', text: 'Charme'},
      ],
      types: ['Places to Be', 'Places to See'],
      contact:{
          title: "PROMOÇÕES",
          subtitle: "Preços especiais por tempo limitado!"
        }
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