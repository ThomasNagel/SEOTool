<template>
  <v-data-table
    :headers="headers"
    :items="products"
    :search="search"
  ></v-data-table>
</template>

<script>
  export default {
    name: 'Table',
    props: {
      headers: Array,
      products: Array
    },
  }
</script>