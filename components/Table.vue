<template>
  <v-simple-table
  color="#DA2627"
   class="mx-auto">
   
    <template v-slot:default
    color="#DA2627"
   class="mx-auto">
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
      <tbody>
        <tr v-for="item in desserts" :key="item.name">
          <td>{{ item.name }}</td>
          <td>{{ item.calories }}</td>
        </tr>
      </tbody>
    </template>
  </v-simple-table>
</template>

