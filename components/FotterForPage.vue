<template>
  <v-footer
    color="#B71C1C"
    padless
  >
    <v-row
      justify="center"
      no-gutters
    >
      <v-btn
        v-for="link in links"
        :key="link"
        color="#FFEBEE"
        text
        
        class="my-2"
      >
        {{ link }}
      </v-btn>
      <v-col
        class="red darken-4 py-4 text-center white--text"
        cols="12"
      >
          </v-col>
    </v-row>
    
  </v-footer>
</template>
<script>
  export default {
    data: () => ({
      links: [
        
        'About Us',
        'Useful Links',
        'Resources',
        'Need Help',
        'Contact Us',
        'Social Media',
       
              
      ],
      
    }),
  }
  </script>
 