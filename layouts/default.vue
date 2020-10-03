<template>
    <!--Your App Starts Here -->
    <v-app id="inspire">
      
      <!--Header -->
      <v-app-bar color="#E22026" dark fixed app>
        <!-- <v-toolbar-title>Application</v-toolbar-title> -->
        <!-- Component Example -->
        
        <Ubilogo/> 
        
        <v-row class="hidden-sm-and-down">
          <!-- tab will be hidden in sm(i pad) and other small screen. It is only for mobile screen -->
          <GlobalNavigation/> 
        </v-row>
        <v-row class="hidden-md-and-up">
          <!-- <v-col sm="8"></v-col> -->
          <v-col sm="1" class="mb-sm-2 ma-sm-2 mb-2 ma-2 mx-0" >
          <!-- mb-margin bellow ma-margin above mx-margin from both side -->
          <hamburger/>
          </v-col>
          </v-row>
        <!-- <v-btn icon>
           
        </v-btn>
         -->
      </v-app-bar> 

      <!-- Body -->
      <v-content light>
      <NavBreadcrumb/>
        <nuxt /> 
      </v-content> 
      
      
     
    <!-- Footer -->
    <v-footer color="indigo" app>
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
      background-color: #9E9E9E;
      color: rgb(255, 255, 255);
    }
  </style>