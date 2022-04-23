<template>
  <v-app>
    <navbar />

    <v-main style="background-color: black;">
      <v-container >
        <nuxt />
      </v-container>
    </v-main>
    <sectionFooter />
  </v-app>
</template>

<script>
  export default {
    data: () => ({
      
    }),
  }
</script>