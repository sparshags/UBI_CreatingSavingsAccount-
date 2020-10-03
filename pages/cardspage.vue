<template>
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    <!--Header -->
    <v-app-bar color="red" dark fixed app>
      <v-toolbar-title></v-toolbar-title>
       <!-- Component such as the logo and the global navigation are linked here -->
      <UbiLogo/> <GlobalNavigation/>
    </v-app-bar>

    <!-- Body -->
    <!-- breadcrumb and all 3 cards are set in columns and cetered -->
    <v-content light>
     
      <nuxt /> 
      
            <v-row justify="center">
        <v-col v-for="i in 3"
    :key=i
    cols="12"
    md="4"
    sx="4">
           <Cards2/> 
           </v-col>
           <v-col v-for="i in 3"
    :key=i
    cols="12"
    md="4"
    sx="4">
             <Cards1/> 
           </v-col>
           <v-col v-for="i in 3"
    :key=i
    cols="12"
    md="4"
    sx="4">
             <Cards3/> 
           </v-col>
          
      </v-row>
      <v-row justify="center">
       <Button/> 
       </v-row>
      
               </v-content>
    
    

  </v-app>
</template>

