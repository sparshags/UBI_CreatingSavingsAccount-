<template>
  <div>
    <!-- format of the breadcrumb is provided -->
    <v-breadcrumbs :items="items" divider="/"></v-breadcrumbs>

   
  </div>
</template>
//the homepage page is linked to the breadcrumb to show that the breadcrumb works unlike the original design of the website 
<script>
  export default {
    data: () => ({
      items: [
        {
          text: 'Home ',
          disabled: false,
          href: 'homePage',
        },
        {
          text: 'Product',
          disabled: false,
          href: 'breadcrumbs_link_1',
        },
        {
          text: 'Personal ',
          disabled: false,
          href: 'breadcrumbs_link_1',
        },
        {
          text: 'Accounts & Deposits',
          disabled: false,
          href: 'breadcrumbs_link_2',
        },
        {
          text: 'Savings Account',
          disabled: true,
          href: 'breadcrumbs_link_2',
        },
        
      ],
    }),
  }
</script>