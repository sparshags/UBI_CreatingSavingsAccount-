<template>
  <v-simple-table >
   <!-- the elements of the table are grouped row wise -->
    <template v-slot:default>
      <thead>
        <tr>
          <th class="text-left">Centers</th>
          <th class="text-left">Without Cheque Book</th>
          <th class="text-left">With Cheque Book</th>
        </tr>
        <tr>
          <th class="text-left">Metro</th>
          <th class="text-left">500</th>
          <th class="text-left">1000</th>
        </tr>
        <tr>
          <th class="text-left">Urban</th>
          <th class="text-left">500</th>
          <th class="text-left">1000</th>
        </tr>
        <tr>
          <th class="text-left">Semi Urban</th>
          <th class="text-left">250</th>
          <th class="text-left">500</th>
        </tr>
        <tr>
          <th class="text-left">Rural</th>
          <th class="text-left">250</th>
          <th class="text-left">500</th>
        </tr>
      </thead>
      <!-- tbody function is used to show blocked text that is not displayed -->
      <tbody>
        <tr v-for="item in desserts" :key="item.name">
          <td>{{ item.name }}</td>
          <td>{{ item.calories }}</td>
        </tr>
      </tbody>
      <!-- table is listed in one of the cards to represent data visually -->
    </template>
  </v-simple-table>
</template>

