<template>
  <Menu>
    <template #default>
      <v-container>
        <!-- Imagen de fondo o hero -->
        <v-row>
          <v-col cols="12">
            <v-img
              src="https://cdn.pixabay.com/photo/2022/04/04/16/42/technology-7111804_640.jpg"
              height="400px"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            >
              <v-container fill-height>
                <v-row align="center" justify="center">
                  <v-col cols="12" md="6">
                    <h1 class="text-h1 white--text">Bienvenido a Mi Gurú</h1>
                    <p class="white--text">
                      Plataforma de aprendizaje y seguimiento de cursos.
                    </p>
                    <v-btn color="primary" dark>Explorar Cursos</v-btn>
                  </v-col>
                </v-row>
              </v-container>
            </v-img>
          </v-col>
        </v-row>

        <!-- Resumen de la plataforma -->
        <v-row justify="center">
          <v-col cols="12" md="8">
            <h2>¿Qué es Mi Gurú?</h2>
            <p>
              Netus accumsan porttitor dis eros mauris platea interdum himenaeos ut, dictumst congue metus ad duis 
              libero penatibus diam consequat, tempor nulla ligula taciti faucibus ullamcorper neque quam. Cursus 
              congue blandit tempor ut taciti gravida, scelerisque vitae dis felis velit, orci conubia augue curae 
              leo. Varius ut nunc et eu penatibus placerat a, ornare dignissim posuere lacus eros pretium litora, 
              turpis massa scelerisque elementum consequat fames. Class natoque commodo molestie lacinia dictumst, 
              cum arcu habitasse magnis eros rutrum, hendrerit dapibus aenean tristique.
            </p>
          </v-col>
        </v-row>
      </v-container>
    </template>
  </Menu>
</template>

<script>
import Menu from '@/components/menu.vue';

export default {
  name: 'Home',
  components: {
    Menu,
  },
};
</script>

<style scoped></style>
