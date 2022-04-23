<template>
<v-row id="store">
    <v-col cols="12">
        <sectionTitle :info="contact" />
      <v-row>
        <v-col cols="12" sm="4">
          <v-card dark>
            <v-img src="https://st3.depositphotos.com/14803258/18680/i/450/depositphotos_186804708-stock-photo-headshot.jpg">
              <v-card-title>Moda Feminina</v-card-title>
            </v-img>
            <v-card-text>
              As melhores combinações para seu guarda-roupa.
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" sm="4">
          <v-card color="#A7121D" dark>
            <v-img src="https://st3.depositphotos.com/12985790/18145/i/450/depositphotos_181451882-stock-photo-portrait-cute-child-bouquet-flowers.jpg">
              <v-card-title class="black--text" >Infantil</v-card-title>
            </v-img>
            <v-card-text>
             Grandes looks para seu pequenino ficar mais lindo ainda.
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" sm="4">
          <v-card dark>
            <v-img src="https://st3.depositphotos.com/14803258/18679/i/450/depositphotos_186793830-stock-photo-happy.jpg">
              <v-card-title>Acessórios</v-card-title>
            </v-img>
            <v-card-text>
             Acessórios de qualidade que a nossa loja garante você cheia de charme.
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
      </v-col>
      <v-col cols="12">
        <v-row>
          <v-col cols="12" sm="4">
            <v-card>
              <v-card-text>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Veritatis quae rerum architecto. Vero distinctio iure aspernatur ut cum rem, numquam ab aliquam aperiam incidunt vel dignissimos. Velit eius et ex.
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellat nisi doloribus repellendus commodi sed autem, assumenda eaque earum cum mollitia repudiandae modi doloremque amet labore corrupti vero reprehenderit quidem non.            
              </v-card-text>
            </v-card>
          </v-col>
          <v-col cols="12" sm="8">
            <v-row>
              <v-col cols="6">
                <v-card>
                  <v-card-text>
                    Ea inventore tempora dicta itaque. Temporibus modi quibusdam pariatur quas eos ratione in iste? Odio aspernatur ipsa culpa ipsam?
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col cols="6">
                <v-card>
                  <v-card-text>
                  Ea inventore voluptate dicta itaque. Temporibus modi quibusdam pariatur quas eos ratione in iste? Odio aspernatur ipsa culpa ipsam?
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col cols="6">
                <v-card>
                  <v-card-text>
                    Ea inventore dsdcdcdsfsvoluptate dicta itaque. Temporibus modi quibusdam pariatur quas eos ratione in iste? Odio aspernatur ipsa culpa ipsam?
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col cols="6">
                <v-card>
                  <v-card-text>
                  t. Quae, voluptatibus. dsdsds sEa inventore tempora voluptate dicta itaque. Temporibus modi quibusdam pariatur quas eos ratione in iste? Odio aspernatur ipsa culpa ipsam?
                  </v-card-text>
                </v-card>
              </v-col>
            </v-row>
            </v-col>
        </v-row>
      </v-col>
</v-row>
    
</template>

<script>
export default {
    data(){
      return{
        contact:{
          title: "NOVIDADES",
          subtitle: "As últimas tendências você encontra aqui"
        }
      }
    }
}
</script>