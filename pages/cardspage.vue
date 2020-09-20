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
      <NavBreadcrumb/>
      <nuxt /> 
            <v-row justify="center">
        <v-col md="3">
           <Cards1/> 
           </v-col>
           <v-col md="3">
             <Cards2/> 
           </v-col>
           <v-col md="3">
             <Cards3/> 
           </v-col>
          
      </v-row>
      <v-row justify="center">
       <Button/> 
       </v-row>
      
               </v-content>
    
    <!-- Footer -->
    <v-footer color="red" app>
      <span class="white--text">&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>

  </v-app>
</template>

