<template>
  <v-form
    ref="form"
    v-model="valid"
    lazy-validation
  >
    

    <v-checkbox textcolor="black"
      v-model="checkbox"
      :rules="[v => !!v || 'You must agree to continue!']"
      label="I have read all the features and understood them."
      required
    ></v-checkbox>

    
    <v-btn
      color="#195289"
      class="mr-4"
      @click="reset"
    >
      Apply
    </v-btn>

    
  </v-form>
</template>

