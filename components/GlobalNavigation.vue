<template>
  <v-card>
    <v-tabs
      v-model="tab"
      background-color="#DA251C" 
       dark
    >
      <v-tab
        v-for="item in items"
        :key="item.tab"
      >
        {{ item.tab }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item
        v-for="item in items" 
        :key="item.tab"
      >
        <v-card flat> 
          <!-- The container used for placing actions for a card -->
          <v-card-text>{{ item.content }}</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
  export default {
    data () {
      return {
        tab: null,
        items: [
          { tab: 'Products', content: 'Tab 1 Content' },//Dropdown box will contain the 6 tabs that is present in all the page 
          { tab: 'Digital Banking', content: 'Tab 2 Content' },
          { tab: 'Investor Relation', content: 'Tab 3 Content' },
          { tab: 'About Us', content: 'Tab 4 Content' },
          { tab: 'Others', content: 'Tab 5 Content' },
          { tab: 'We Care', content: 'Tab 6 Content' },
          
        ],
      }
    },
  }
</script>