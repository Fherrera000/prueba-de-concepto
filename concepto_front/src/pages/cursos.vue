<template>
    <Menu>
      <template #default>
        <v-container>
          <v-row>
            <v-col cols="12" md="4">
              <v-card>
                <v-img
                  src="https://img.freepik.com/vector-gratis/concepto-diseno-web-dibujado-mano_23-2147839737.jpg"
                  height="200px"
                ></v-img>
                <v-card-title>Curso de capacitación 01</v-card-title>
                <v-card-subtitle>primer curso</v-card-subtitle>
                <v-card-text>
                    Lorem ipsum dolor sit amet consectetur adipiscing elit vehicula ac etiam, condimentum vulputate 
                    dignissim conubia per non natoque mattis hac placerat, neque commodo maecenas tempor vel nullam 
                    netus iaculis convallis. Condimentum porttitor per dis nostra tempor convallis litora, ullamcorper 
                    mauris non nascetur nisi semper penatibus, sed curabitur id ultrices fermentum habitant. 
                    Justo suscipit nunc laoreet venenatis sodales purus turpis nisl, ridiculus montes faucibus 
                    dignissim dapibus in per dui, lacinia aenean cum congue imperdiet vel eleifend
                </v-card-text>
                <v-card-actions>
                  <v-btn color="primary">Seleccionar</v-btn>
                </v-card-actions>
              </v-card>
            </v-col>
  
            <v-col cols="12" md="4">
              <v-card>
                <v-img
                  src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEirqFAw-J6wyzqlow1SqgB5HCu6KnHzNAVq1vYz0A0TXzZ50LyY4oPiDmmooZgglSYE8sO1jR51gfmFK2qdCUZ-sOOwyNKA8gSVmE70gIp9QF2YUPkl1gpJRfmU2mpA5932tugBP8JZzbQv/s1600/Tecnologia+%25281%2529.jpg"
                  height="200px"
                ></v-img>
                <v-card-title>Curso de capacitacion 02</v-card-title>
                <v-card-subtitle>segundo curso</v-card-subtitle>
                <v-card-text>
                    Fusce dictum pellentesque diam auctor lobortis laoreet et vivamus massa nulla 
                    tempus pharetra feugiat natoque, class at hendrerit nisl eros accumsan taciti facilisi nullam eu 
                    hac aptent magnis. Non felis libero tortor integer ut aliquet tempus, lacinia leo sollicitudin 
                    mi platea erat, lobortis congue eu quis dui nunc. Ultricies posuere mattis enim nullam magna in felis, 
                    libero phasellus lacinia penatibus scelerisque 
                    natoque venenatis duis, cursus euismod vulputate eleifend faucibus ridiculus.
                </v-card-text>
                <v-card-actions>
                  <v-btn color="primary">Seleccionar</v-btn>
                </v-card-actions>
              </v-card>
            </v-col>
  
            <v-col cols="12" md="4">
              <v-card>
                <v-img
                  src="https://www.fundacionaquae.org/wp-content/uploads/2020/09/tecnologia-educacion-1024x684.jpg"
                  height="200px"
                ></v-img>
                <v-card-title>Curso de capacitacion 03</v-card-title>
                <v-card-subtitle>tercer curso</v-card-subtitle>
                <v-card-text>
                    Praesent porttitor urna purus parturient mus sem hendrerit senectus bibendum 
                    eu vivamus lacinia, aptent fermentum taciti ad volutpat dictum sed sociosqu nulla tortor 
                    suscipit class fringilla, mauris pretium blandit vitae posuere per vehicula nec augue lectus 
                    aliquet. Felis rhoncus non molestie tempus sed etiam vel ornare convallis, mi diam potenti ante 
                    mus pharetra augue aptent, quam tristique purus interdum vehicula nisl nullam proin. Accumsan 
                    ridiculus semper sodales congue fermentum facilisis augue vulputate, eros nascetur curabitur 
                    porttitor mattis morbi.
                </v-card-text>
                <v-card-actions>
                  <v-btn color="primary">Seleccionar</v-btn>
                </v-card-actions>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      </template>
    </Menu>
  </template>
  
  <script>
  import Menu from '@/components/Menu.vue';
  
  export default {
    components: {
      Menu,
    },
  };
  </script>