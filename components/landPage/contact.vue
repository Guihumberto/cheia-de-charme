<template>
  <v-row id="contact">
      <sectionTitle :info="contact" />
      <v-col cols="12" sm="7">
        <div class="containerJJJ">
          <iframe class="responsive-iframe" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3985.9219181716217!2d-44.238149685244046!3d-2.532376698154745!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x7f691312867d40b%3A0x82cd18254b0564f1!2sEasy%20Confeitaria!5e0!3m2!1spt-BR!2sbr!4v1650655978682!5m2!1spt-BR!2sbr"></iframe>
        </div>
        </v-col>
      <v-col cols="12" sm="5">
          <sectionTitle :info="adrress" />
          <v-card>
            <v-card-text>
              Rua XXX, Bairro Vinhais, <br>
              São Luis - MA, CEP: 65063-010 <br>
              Ponto de Referência:
            </v-card-text>
          </v-card>
          <sectionTitle :info="sociais" />
          <v-card class="mt-1">
            <v-card-text>
              Telefone <br>
              WhatsAPP <br>
              E-mail <br>
              Instagram
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
          subtitle: "Endereço, contato e redes sociais"
        },
        sociais:{
          title: "Contato",
          subtitle: null
        },
        adrress:{
          title: "Endereço",
          subtitle: null
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