<template>
    <v-app>
      <!-- Barra de navegación -->
      <v-app-bar app color="primary" dark>
        <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
        <v-toolbar-title>Mi Gurú</v-toolbar-title>
      </v-app-bar>
  
      <!-- Drawer de navegación -->
      <v-navigation-drawer v-model="drawer" temporary>
        <v-list>
          <v-list-item link to="/">
            <v-list-item-content>
              <v-list-item-title>Página Principal</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item link to="/cursos">
            <v-list-item-content>
              <v-list-item-title>Cursos</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item link to="/dashboard">
            <v-list-item-content>
              <v-list-item-title>Dashboard</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item link to="/reportes">
            <v-list-item-content>
              <v-list-item-title>Reportes</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
  
      <!-- Contenido principal -->
      <v-main>
        <slot />
      </v-main>

    </v-app>
  </template>
  
  <script>
  export default {
    name: 'Menu',
    data() {
      return {
        drawer: false,
      };
    },
  };
  </script>
  
  <style scoped>
  /* Estilos opcionales */
  </style>