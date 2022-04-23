<template>
    <v-row id="about" class="mb-2">
        <sectionTitle :info="contact" />
        <v-col cols="12">
            <v-card color= '#952175' dark>
            <v-card-title>
                CHEIA DE CHARME
            </v-card-title>
            <v-card-text style="text-align: justify;">
              A Loja Cheia de Charme nasceu em 2011, e vem fazendo histórias e participando de momentos incríveis na vida de nossos clientes 
              que nos acompanham há mais de 10 anos. Venha fazer parte dessa nossa histórias.!!! Aqui você encontra as melhores promoções! Aproveite nossas ofertas: Roupas infantis, como blusas, conjuntos e Body e temos roupas femininas blusas, calças e shorts com 20%, 30% , 40% e até 50% de desconto à vista.
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
          title: "QUEM SOMOS NÓS",
          subtitle: "Nossa história",
          icon: 'mdi-information-outline'
        }
      }
    }
}
</script>