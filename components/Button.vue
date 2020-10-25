<template>
<!-- The validate button has been taken from a form and adjusted according to layout -->
<!-- valid means a function has to take place in order fro the button to get activated -->
  <v-form
    ref="form"
    v-model="valid"
    lazy-validation
  >
    
<!-- the below function defines the task to be completed in order to validate the button  -->
    <v-checkbox textcolor="black"
      v-model="checkbox"
      :rules="[v => !!v || 'You must agree to continue!']"
      label="I have read all the features and understood them."
      required
    ></v-checkbox>
<!-- color of the button has been changed -->
    
    <v-btn
      color="#195289"
      class="mr-4"
      @click="validate"
    >
      Apply
    </v-btn>

    
  </v-form>
</template>
<script>
var vm = new validate({
  data: {
    // declare message with an empty value
    message: 'You must agree to continue!'
  },
  template: '<div>{{You must agree to continue!}}</div>'
})
// set `message` later
vm.message = 'You must agree to continue!'
</script>

