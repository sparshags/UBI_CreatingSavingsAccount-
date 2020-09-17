<template>
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    <!--Header -->
    <v-app-bar color="red" dark fixed app>
      <v-toolbar-title>Application</v-toolbar-title>
       <!-- Component Example -->
      <UbiLogo/> <GlobalNavigation/>
    </v-app-bar>

    <!-- Body -->
    <v-content light>
      <nuxt /> <Carousel/>
    </v-content>
    
    <!-- Footer -->
    <v-footer color="indigo" app> <FooterDown/>
      <span class="white--text">&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>

  </v-app>
</template>

<script>
export default {}
</script>

<style> 
  .white--text {
    border: 1px solid;
  }

   #inspire {
    background-color: white;
    color: black; 
  }
</style>