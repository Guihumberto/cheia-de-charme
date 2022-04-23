<template>
  <v-row id="contact">
      <sectionTitle :info="contact" />
      <v-col cols="12" sm="7">
        <div class="containerJJJ">
          <iframe class="responsive-iframe" src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d3985.9796558590256!2d-44.2513733!3d-2.513541!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x475047a6e8b12d84!2zMsKwMzAnNDguOCJTIDQ0wrAxNScwNC45Ilc!5e0!3m2!1spt-BR!2sbr!4v1650720966646!5m2!1spt-BR!2sbr"></iframe>
        </div>
        </v-col>
      <v-col cols="12" sm="5">
          <sectionTitle :info="address" />
          <v-card>
            <v-card-text>
              Av. três, nº 06, Bairro Vinhais, <br>
              São Luis - MA, CEP: 65071-020 <br>
              Ponto de Referência: em  frente a UEB: BALÃO MÁGICO/COLEGIO: Prof NASCIMENTO DE MORAIS
            </v-card-text>
          </v-card>
          <sectionTitle :info="sociais" />
          <v-card class="mt-1">
            <v-card-text>
              <v-row>
                <v-col cols="6">
                  <v-icon small>mdi-cellphone</v-icon> Telefone:<br>
                  <v-icon small>mdi-whatsapp</v-icon> WhatsAPP: <br>
                  <v-icon small>mdi-email</v-icon> E-mail: <br>
                  <v-icon small>mdi-instagram</v-icon> Instagram:
                </v-col>
                <v-col cols="6">
                  98 98844-2459 <br>
                  98 98844-2459 <br>
                  cheiadecharme_loja@ <br>
                  cheiadecharme_loja <br>
                </v-col>
              </v-row>
            </v-card-text>
          </v-card>
      </v-col>
  </v-row>
    
</template>

<script>
export default {
    data(){
      return{
        contact:{
          title: "CONTATO",
          subtitle: "Endereço, contato e redes sociais",
          icon: 'mdi-cellphone'
        },
        sociais:{
          title: "Contato",
          subtitle: null,
          icon: 'mdi-cellphone'
        },
        address:{
          title: "Endereço",
          subtitle: null,
          icon: 'mdi-map-marker-outline'
        },
      }
    }
}
</script>

<style scoped>
.containerJJJ {
  position: relative;
  overflow: hidden;
  width: 100%;
  padding-top: 56.25%; /* 16:9 Aspect Ratio (divide 9 by 16 = 0.5625) */
}

/* Then style the iframe to fit in the container div with full height and width */
.responsive-iframe {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  width: 100%;
  height: 100%;
}
</style>