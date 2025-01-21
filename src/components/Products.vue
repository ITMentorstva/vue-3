<template>

  <ul>
    <li v-for="phone in phones" :key="phone.name">
      {{ phone.name }} - Price: {{ phone.price }} - Stock: {{ phone.amount }}
    </li>
  </ul>
  
</template>

<script>
  export default {

    name: 'Products',

    data() {
      return {
        phones: [
          { name: 'iPhone 15', price: 1500, amount: 32 },
          { name: 'Samsung Galaxy S23', price: 1200, amount: 0 },
          { name: 'Google Pixel 8', price: 900, amount: 15 },
          { name: 'OnePlus 11', price: 800, amount: 0 },
          { name: 'Sony Xperia 5 IV', price: 1000, amount: 8 },
          { name: 'Huawei P50 Pro', price: 1100, amount: 5 },
          { name: 'Xiaomi Mi 13', price: 700, amount: 20 },
          { name: 'LG Velvet', price: 650, amount: 0 },
          { name: 'Motorola Edge 40', price: 750, amount: 12 },
          { name: 'Nokia XR20', price: 600, amount: 7 }
        ]
      }
    },

    beforeCreate() {
      console.log("Before create")
    },

    created() {
      console.log("Created")
    },

    beforeMount() {
      console.log('Before mount')
    },

    mounted() {
      console.log('Mounted')
    }
  }
</script>