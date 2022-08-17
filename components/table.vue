<template>
  <v-card>
    <v-card-title>
      <v-text-field
        v-model="search"
        append-icon="mdi-magnify"
        label="Search"
        single-line
        hide-details
      ></v-text-field>
    </v-card-title>
    <v-data-table
      :headers="headers"
      :items="products"
      :search="search"
    ></v-data-table>
  </v-card>
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