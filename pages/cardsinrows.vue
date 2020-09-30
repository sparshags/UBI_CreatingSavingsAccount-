<template>
<v-container class="10">
    <v-layout row>
          
    <v-col
    v-for="i in 3"
    :key=i
    cols="12"
    md="4"
    >

      <v-card
         class="pa-md-4 pa-sm-4 pa-xs-4 mx-lg-auto mx-sm-auto"
    color="blue"
    width="150px" >
        <v-card-text>
          mid Centered
        </v-card-text>
      </v-card>

    </v-col>
    </v-layout>

  <v-layout row
    no-gutters
    >
    <v-col
    v-for="j in 2"
    :key=j
    cols="12"
    md="6"
    >

      <v-card
        class="purple lighten-3 pa-3"
      >
        <v-card-text>
          Centered
        </v-card-text>
      </v-card>

    </v-col>
     
    </v-layout>
</v-container>
  </template>