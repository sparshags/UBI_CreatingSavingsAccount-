<template>
  <div>
    <v-breadcrumbs :items="items" divider="-"></v-breadcrumbs>

   
  </div>
</template>

<script>
  export default {
    data: () => ({
      items: [
        {
          text: 'Home  /',
          disabled: false,
          href: 'homePage',
        },
        {
          text: 'Product  /',
          disabled: false,
          href: 'breadcrumbs_link_1',
        },
        {
          text: 'Personal  /',
          disabled: false,
          href: 'breadcrumbs_link_1',
        },
        {
          text: 'Accounts & Deposits  /',
          disabled: false,
          href: 'breadcrumbs_link_2',
        },
        {
          text: 'Savings Account  /',
          disabled: true,
          href: 'breadcrumbs_link_2',
        },
        
      ],
    }),
  }
</script>