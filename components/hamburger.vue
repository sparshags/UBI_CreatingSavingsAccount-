<template>
  <div class="text-center">
    <!-- open on click command allows the card to show options when clicked -->
    <v-menu
      open-on-click
      top
      offset-y>
      <!-- the slot is activated when clicked -->
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="#E22026"
          dark
          v-bind="attrs"
          v-on="on"
          height="48"
          width="20">
          MENU
        </v-btn>
      </template>

      <v-list>
        <v-list-item
          v-for="(item, index) in items"
          :key="index"
        >
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>
  </div>
</template>

<script>
  export default {
    data: () => ({
      items: [
        { title: 'PRODUCTS' },
        { title: 'DIGITAL BANKING' },
        { title: 'INTERNATIONAL RELATIONS' },
        { title: 'WE CARE' },
        { title: 'CONTACT US' },
        { title: 'ABOUT US' },
      ],
    }),
  }
</script>
