<template>
  <div id="app">
    <Header title="Homming Programming Proficiency Test! 👨🏻‍💻"/>
    <Table />
    <Footer createdBy="Made by Friosn with 💚 and 🧉"/>
  </div>
</template>

<script>
import { users, propertyTypes, properties } from '@/mocks/api';

import Footer from '@/components/Footer.vue';
import Header from '@/components/Header.vue';
import Table from '@/views/Table.vue';

export default {
  name: 'App',
  data: () => ({
    users,
    propertyTypes,
    properties,
  }),
  components: { Header, Footer, Table },
};
</script>

<style>
  #app {
    height: 90vh;
    width: 100%;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
  }
</style>
