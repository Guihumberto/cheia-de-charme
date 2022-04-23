<template>
    <v-app-bar app flat dark color="#111111">
      <v-container style="max-width: 1080px" class="py-0 fill-height">
        <v-btn icon>
          <v-icon color="#A7121D">mdi-snake</v-icon>
        </v-btn>

        CHEIA DE CHARME

        <v-spacer></v-spacer>

        <v-btn text @click="scroll('store')">Loja</v-btn>
        <v-btn text @click="scroll('sales')">Promoções</v-btn>
        <v-btn text @click="scroll('about')"> Sobre</v-btn>
        <v-btn text @click="scroll('contact')">Contato</v-btn>
      </v-container>
    </v-app-bar>
</template>

<script>
export default {
  methods: {
    scroll(refName) {
      const element = document.getElementById(refName);
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>

<style lang="scss" scoped>

</style>