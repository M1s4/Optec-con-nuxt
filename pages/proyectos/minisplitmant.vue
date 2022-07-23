<template>
  <v-container fluid class="ma-0 pa-0">
    <btn-back />
    <v-container fluid class="ma-0 pa-0 ">
      
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
              Mantenimiento preventivo a minisplit
            </v-card-subtitle>
          </v-card>
        </v-img>
      </v-card>

      <v-card
        width="100%"
        light
        elevation="0"
        class="pt-10 pb-5 px-3 rounded-0"
      >
        <p class="font-weight-black text-h6 text-md-h5">
          Mantenimiento preventivo a minisplit
        </p>

        <p class="pt-2 font-weight-bold text-subtitle-1 grey--text mb-0">
          INFORMACION DE PROYECTO
        </p>
        <p class="pt-3 grey--text text-body-1 text-left font-weight-normal t">
          Sin el mantenimiento adecuado, tu minisplit enfriará menos y consumirá más energía eléctrica.
          Para prolongar su vida útil, aquí te decimos cómo limpiarlo paso a paso.
        </p>
       
      </v-card>

      <v-card elevation="0" class="py-10 px-3 pt-2 rounded-0" light>
        <p class="font-weight-bold text-subtitle-1  pb-2">
          LO QUE HICIMOS
        </p>
        
        <p class="grey--text text-subtitle-2 ">
           limpieza de los serpentines (evaporador y condensador).
        </p>
        <p class="grey--text text-subtitle-2 ">
          Limpiar y revisar los abanicos del evaporador y del condensador
        </p>
        <p class="grey--text text-subtitle-2 ">
          Revisar las señales emitidas por la tarjeta electrónica.
        </p>
        <p class="grey--text text-subtitle-2 ">
          Revisar la presión del refrigerante.
        </p>
        <p class="grey--text text-subtitle-2 ">
          Analizar el consumo eléctrico.
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
        <v-card class=" pt-5" elevation="0">
          <v-btn
            color="#FFD763"
            class="
              font-weight-normal
              rounded-0
              py-6
              text-lowercase text--grey-darken-4
            "
            width="100%"
            href="https://api.whatsapp.com/send?phone=3221884814&text=Hola!%20"
            target="_blank"
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
          img: "tres.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MinisplitMCP.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MinisplitMCP02.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MinisplitMCP03.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MinisplitMCP04.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MinisplitMCP05.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MinisplitMCP06.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MinisplitMCP07.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MinisplitMCP08.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "MinisplitMCP09.jpg",
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