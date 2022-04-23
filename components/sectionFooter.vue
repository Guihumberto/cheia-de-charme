<template>
  <v-footer
    dark
    padless
  >
    <v-card
      flat
      tile
      color="#A7121D"
      class="lighten-1 white--text text-center"
      width="1980"
    >
      <v-card-text>
        <v-btn
          v-for="(icon, index) in icons"
          :key="index"
          class="mx-4 white--text"
          icon
          target="_blank"
          :href="icon.url"
        >
        
          <v-icon size="24px">
            {{ icon.icon }}
          </v-icon>
        </v-btn>
      </v-card-text>

      <v-card-text class="white--text pt-0">
            Av. três, nº 06, Bairro Vinhais, <br>
            São Luis - MA, CEP: 65071-020 <br>
            em  frente a UEB: BALÃO MÁGICO/COLEGIO: Prof NASCIMENTO DE MORAIS
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>Cheia de Charme</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>
<script>
  export default {
    data: () => ({
      icons: [
        {icon:'mdi-whatsapp', url:''},
        {icon:'mdi-email', url:''},
        {icon:'mdi-instagram', url:'https://instagram.com/cheiadecharme_loja?igshid=YmMyMTA2M2Y='},
      ],
    }),
  }
</script>