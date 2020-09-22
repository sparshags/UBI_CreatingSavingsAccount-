<template>
<v-container>
  <v-row>
    <v-col v-for="i in 3"
    :key=i
    cols="12"
    md="4"
    sx="4">
    <v-card
    class="pa-md-4 pa-sm-4 pa-xs-4 mx-lg-auto mx-sm-auto"
    color="blue"
    width="150px">
    <v-card-text class="red--text">
    Cards
    </v-card-text>
    </v-card>
    </v-col>
  </v-row>
</v-container>
</template>