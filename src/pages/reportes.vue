<template>
    <Menu>
      <template #default>
        <v-container>

          <v-row>
            <v-col cols="12" md="6">
              <v-select
                :items="cursos"
                v-model="cursoSeleccionado"
                label="Seleccione un curso"
              ></v-select>
            </v-col>
            <v-col cols="12" md="6">
              <v-select
                :items="usuarios"
                v-model="usuarioSeleccionado"
                label="Seleccione un usuario"
              ></v-select>
            </v-col>
          </v-row>
  
          <v-row>
            <v-col cols="12">
              <v-btn color="primary" @click="generarReporte">Generar Reporte</v-btn>
            </v-col>
          </v-row>
  

          <v-row v-if="reporteGenerado">
            <v-col cols="12">
              <v-card>
                <v-card-title>Reporte de {{ usuarioSeleccionado }}</v-card-title>
                <v-card-text>
                  <p>Curso: {{ cursoSeleccionado }}</p>
                  <p>Fecha de Inicio: {{ fechaInicio }}</p>
                  <p>Fecha de Finalización: {{ fechaFinalizacion }}</p>
                  <p>Calificación: {{ calificacion }}</p>
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
  
          <v-row>
            <v-col cols="12">
              <v-btn color="primary" @click="imprimirReporte">Imprimir Reporte</v-btn>
            </v-col>
          </v-row>
        </v-container>
      </template>
    </Menu>
  </template>
  
  <script>
  import Menu from '@/components/Menu.vue';
  
  export default {
    name: 'Reportes',
    components: {
      Menu,
    },
    data() {
      return {
        cursos: ['Curso 01', 'Curso 02', 'Curso 03'],
        usuarios: ['Usuario 1', 'Usuario 2', 'Usuario 3'],
        cursoSeleccionado: '',
        usuarioSeleccionado: '',
        reporteGenerado: false,
        fechaInicio: '',
        fechaFinalizacion: '',
        calificacion: '',
      };
    },
    methods: {
      generarReporte() {
        this.reporteGenerado = true;
        this.fechaInicio = '2025-01-01';
        this.fechaFinalizacion = '2025-01-31';
        this.calificacion = 'Aprobado';
      },
      imprimirReporte() {
        window.print();
      },
    },
  };
  </script>
  
  <style scoped>
  /* Estilos opcionales */
  </style>