<template>
  <v-container class="grey lighten-5">
    <v-row no-gutters>
      <!-- v for is loopin -->
      <!-- sm is small and md is midum it is imp for the website to adapt to change in device -->
      <v-col
        v-for="n in 3"
        :key="n"
        cols="12"
        sm="2"
        md="4"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          One of three columns
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>