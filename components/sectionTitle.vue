<template>
      <v-col cols="12" sm="12" class="d-flex justify-space-between">
            <div>
                  
                  <h4 v-if="info.title" class="white--text"> <span v-if="!info.icon" class="tagred"></span>
                  <v-icon small v-if="info.icon" color="white"> {{info.icon}} </v-icon> {{info.title}}</h4>
                  <p v-if="info.subtitle" class="grey--text">{{info.subtitle}} </p>
            </div>
            <v-btn v-if="info.btn" :to="info.url" dark color="#A7121D">{{info.btnTitle}}</v-btn>
      </v-col>
</template>

<script>
export default {
      props:{
            info:Object
      }
}
</script>
