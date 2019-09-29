<template>
  <v-app>
    <app-header></app-header>

    <v-content>
      <v-card class="d-flex justify-center transparent elevation-0 pa-4">
        <servers class="flex-grow-1 mr-2"></servers>
        <server-details class="flex-grow-1 ml-2"></server-details>
      </v-card>
      
    </v-content>
    <app-footer></app-footer>
  </v-app>
</template>

<script>
import AppHeader from './components/Header';
import AppFooter from './components/Footer';
import Servers from './components/Servers';
import ServerDetails from './components/ServerDetails';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
    Servers,
    ServerDetails
  },
  data: () => ({
    //
  }),
};
</script>
