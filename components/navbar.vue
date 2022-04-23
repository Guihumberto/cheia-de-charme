<template>
    <v-app-bar app flat dark color="#111111">
      <v-container style="max-width: 1080px" class="">
        <v-tabs centered>
          <v-tab>
            <v-btn text @click="scroll('header')">
              <v-icon small color="#A7121D" class="mr-1">mdi-snake</v-icon>
              cheia de charme</v-btn>
          </v-tab>
          <v-tab>
            <v-btn text @click="scroll('store')">Loja</v-btn>
          </v-tab>
          <v-tab>
            <v-btn text @click="scroll('sales')">Promoções</v-btn>
          </v-tab>
          <v-tab>
            <v-btn text @click="scroll('about')"> Sobre</v-btn>
          </v-tab>
          <v-tab>
            <v-btn text @click="scroll('contact')">Contato</v-btn>
          </v-tab>
      </v-tabs>
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