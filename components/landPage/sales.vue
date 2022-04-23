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
          <v-card>
            <v-img
              :src="photo.src"
              height="300px"
            >
              <span
                class="text-h5 white--text pl-4 pt-4 d-inline-block"
                v-text="photo.text"
              ></span>
            </v-img>

            <v-card-actions class="white justify-center">
              <v-btn
                v-for="(social, i) in socials"
                :key="i"
                :color="social.color"
                class="white--text"
                fab
                icon
                small
              >
                <v-icon>{{ social.icon }}</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
</template>

<script>
  export default {
    data: () => ({
      photos:[
        {src: '2.jpeg', text: 'Good'},
        {src: '3.jpeg', text: 'Best'},
        {src: '4.jpeg', text: 'Finest'},
        {src: '5.jpeg', text: 'Good'},
        {src: '6.jpeg', text: 'Best'},
        {src: '7.jpeg', text: 'Finest'},
      ],
      types: ['Places to Be', 'Places to See'],
      socials: [
        {
          icon: 'mdi-facebook',
          color: 'indigo',
        },
        {
          icon: 'mdi-whatsapp',
          color: 'cyan darken-1',
        },
        {
          icon: 'mdi-instagram',
          color: 'red lighten-3',
        },
      ],
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
    },
  }
</script>