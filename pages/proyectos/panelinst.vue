<template>
  <v-container fluid class="ma-0 pa-0">
    <btn-back />

    <v-container fluid class="ma-0 pa-0">
      <v-card width="100%" color="red" height="130" class="text-center">
        <v-img
          class="white--text align-center rounded-0"
          height="100%"
          :src="require(`../../assets/images/backproyectos.jpg`)"
          position="center 60%"
          gradient="rgba(21,22,24,.2), rgba(21,22,24.1)"
        >
          <v-card class="text-center" color="transparent" elevation="0">
            <v-card-subtitle
              class="text-caption pb-0 mb-0 font-weight-black white--text"
            >
              Ultimos proyectos
            </v-card-subtitle>
            <v-card-subtitle
              class="text-subtitle-2 pa-0 pt-2 white--text font-weight-normal"
            >
              Mantenimiento preventivo y predictivo a sistema de paneles solares
            </v-card-subtitle>
          </v-card>
        </v-img>
      </v-card>

      <v-card
        width="100%"
        light
        elevation="0"
        class="pt-13 rounded-0 px-5 pb-4"
      >
        <p class="font-weight-black text-h6 text-md-h5">
          Mantenimiento preventivo y predictivo a sistema de paneles solares
        </p>

        <p class="pt-2 font-weight-bold text-subtitle-1 grey--text mb-0">
          INFORMACION DE PROYECTO
        </p>
        <p class="pt-3 grey--text text-body-1 text-left font-weight-normal t">
          Las ventajas del mantenimiento preventivo son, entre otras: detectar fallos repetitivos,
          disminuir los puntos muertos por paradas, aumentar la vida útil de equipos, 
          disminuir coste de reparaciones, y detectar puntos débiles en la instalación.
        </p>
        
      </v-card>

      <v-card elevation="0" class="px-5 pt-5 rounded-0" light>
        <p class="font-weight-bold text-subtitle-1 pr-15 mb-2">
         LO QUE HICIMOS
        </p>

        <p class="grey--text text-body-1">
          Limpieza o cambios de filtros de aire
        </p>
        <p class="grey--text text-body-1">
          Limpieza de rejillas protectoras en entradas y salidas de aire.

        </p>
        <p class="grey--text text-body-1">
          Limpieza de ventiladores externos.

        </p>
        <p class="grey--text text-body-1">
          Comprobar sellado de la carcasa.
        </p>
        <p class="grey--text text-body-1">
          Inspección de polvo, suciedad, humedad en el interior de los inversores.
        </p>
        <p class="grey--text text-body-1">
          Inspección de polvo, suciedad, humedad en el interior de los inversores.
        </p>
        <p class="grey--text text-body-1">
          Comprobar la limpieza de ventiladores.
        </p>
        <v-row justify="space-around">
          <v-card width="100%" elevation="0">
            <v-slide-group class="pa-4" active-class="success">
              <v-slide-item
                v-for="(item, i) in nosotros"
                :key="i"
                v-slot="{ active, toggle }"
              >
                <v-card
                  :color="active ? undefined : 'grey lighten-1'"
                  class="mr-2 rounded-0"
                  height="150"
                  width="180"
                  @click="toggle"
                >
                  <v-img
                    width="100%"
                    height="100%"
                    :src="require(`../../assets/images/${item.img}`)"
                  />
                  <v-img />
                </v-card>
              </v-slide-item>
            </v-slide-group>
          </v-card>
        </v-row>
        <v-card class="d-flex justify-center py-5" elevation="0">
          <v-btn
            color="#FFD763"
            class="
              font-weight-normal
              rounded-0
              py-6
              text-lowercase text--grey-darken-4"
            href="https://api.whatsapp.com/send?phone=3221884814&text=Hola!%20" 
            target="_blank"
            width="100%"
          >
            <v-icon left> mdi-cellphone-text </v-icon>
            pedir cotizacion
          </v-btn>
        </v-card>
      </v-card>
      
    </v-container>
  </v-container>
</template>

<script lang="ts">
import BtnBack from "../../components/BtnBack.vue";

export default {
  data() {
    return {
      nosotros: [        
        {
          nombre: "",
          img: "MantPanel01.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel02.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "panelS.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel012.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel013.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel03.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel04.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel05.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel06.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel07.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel08.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel09.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel010.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MantPanel011.jpg",
          data: "",
        },
        

      ],
    };
  },

  components: {
    BtnBack,
  },
};
</script>

<style>
</style>