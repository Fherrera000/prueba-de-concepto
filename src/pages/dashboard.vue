<template>
    <Menu>
      <template #default>
        <v-container>

          <v-row justify="center">
            <v-col cols="12" class="text-center">
              <h1>Estadisticas de cursos</h1>
            </v-col>
          </v-row>
  

          <v-row>
            <v-col cols="12" md="4">
              <v-card outlined>
                <v-card-title>Curso 01</v-card-title>
                <v-card-text class="text-center">
                  <v-progress-circular
                    :value="curso01"
                    color="blue"
                    size="100"
                    width="10"
                  >
                    {{ curso01 }}%
                  </v-progress-circular>
                  <p>Usuarios inscritos: {{ inscritosCurso01 }}</p>
                </v-card-text>
              </v-card>
            </v-col>
  
            <v-col cols="12" md="4">
              <v-card outlined>
                <v-card-title>Curso 02</v-card-title>
                <v-card-text class="text-center">
                  <v-progress-circular
                    :value="curso02"
                    color="green"
                    size="100"
                    width="10"
                  >
                    {{ curso02 }}%
                  </v-progress-circular>
                  <p>Usuarios inscritos: {{ inscritosCurso02 }}</p>
                </v-card-text>
              </v-card>
            </v-col>
  
            <v-col cols="12" md="4">
              <v-card outlined>
                <v-card-title>Curso 03</v-card-title>
                <v-card-text class="text-center">
                  <v-progress-circular
                    :value="curso03"
                    color="red"
                    size="100"
                    width="10"
                  >
                    {{ curso03 }}%
                  </v-progress-circular>
                  <p>Usuarios inscritos: {{ inscritosCurso03 }}</p>
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      </template>
    </Menu>
  </template>
  
  <script>
  import Menu from '@/components/menu.vue';
  
  export default {
    components: {
      Menu,
    },
    data() {
      return {
        curso01: 75,
        curso02: 50,
        curso03: 90,
        inscritosCurso01: 120,
        inscritosCurso02: 80,
        inscritosCurso03: 150,
      };
    },
  };
  </script>
  
  <style scoped>
  h1 {
    font-size: 2rem;
    margin-bottom: 20px;
  }
  </style>