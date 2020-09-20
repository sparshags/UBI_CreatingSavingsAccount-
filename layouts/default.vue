<template>
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    <!--Header -->
    <v-app-bar color="red" dark fixed app>
      <v-toolbar-title></v-toolbar-title>
       <!-- Component Example -->
      <UbiLogo/> <GlobalNavigation/>  
    </v-app-bar>

    <!-- Body -->
    <v-content light>
      
      <nuxt /> 
            
          
          
               </v-content>
    
    <!-- Footer -->
    <!-- footer is added and its size and color is defined. it is also justified to the center -->
    <v-footer color="#DA2627" app>
      <v-row justify="center">
      <img
    class="footer"
    alt="footer"
    src="footer.png"
  >
  <style>
.footer {
  height: 170px;
  width: 700px;
}
</style>
      </v-row>
    </v-footer>

  </v-app>
</template>

<script>
export default {}
</script>

<style> 
  .blue--text {
    border: 1px solid;
  }

   #inspire {
    background-color: rgb(204, 204, 204);
    color: black; 
  }
</style>