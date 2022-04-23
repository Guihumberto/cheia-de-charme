<template>
      <v-col cols="12" sm="12">
            <h4 v-if="info.subtitle" class="white--text">{{info.title}}</h4>
            <p v-if="info.subtitle" class="grey--text">{{info.subtitle}} </p>
      </v-col>
</template>

<script>
export default {
      props:{
            info:Object
      }
}
</script>
