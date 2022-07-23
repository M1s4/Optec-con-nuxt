<template>
  <v-container fluid class="ma-0 pa-0">
    <v-card elevation="0" class="px-3 pt-10 pb-7 rounded-0" light>
      <p class="cyan--text font-weight-bold text-caption">
        <v-icon left color="cyan">mdi-minus</v-icon>
        SOBRE NOSOTROS
      </p>
      <p class="font-weight-black text-h5 pr-15 mb-0">
        OPTEC Proyectos Y Mantenimiento
      </p>
      <p class="font-weight-bold text-caption grey--text">
        nos esforzamos por alcanzar la excelencia.
      </p>

      <p class="grey--text text-body-1">
        En <strong>OPTEC</strong> somos una empresa que contamos con un equipo de Ingenieros experimentados, calificados y confiables que
        brinda soluciones integrales de ingenieria, proyectos de obra eléctrica, mantenimiento industrial y residencial para propiedades residenciales y comerciales.               
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
                height="200"
                width="180"
                @click="toggle"
              >
                <img
                  width="100%"
                  height="100%"
                  :src="require(`../assets/images/${item.img}`)"
                />
                <img />
              </v-card>
            </v-slide-item>
          </v-slide-group>
        </v-card>
      </v-row>
      <v-card class="d-flex justify-center mt-5" elevation="0">
        <v-btn
          color="#FFD763"
          class="
            font-weight-normal
            rounded-0
            py-6
            text-lowercase text--grey-darken-4
          "
          width="100%"
          href="https://api.whatsapp.com/send?phone=3221807041&text=Hola!%20"
          target="_blank"
        >
          <v-icon left> mdi-cellphone-text </v-icon>
          pedir cotizacion
        </v-btn>
      </v-card>
    </v-card>
  </v-container>
</template>

<script lang="ts">
export default {
  data() {
    return {
      tags: [
        "Work",
        "Home Improvement",
        "Vacation",
        "Food",
        "Drawers",
        "Shopping",
        "Art",
        "Tech",
        "Creative Writing",
      ],
      nosotros: [
        {
          nombre: "",
          img: "NUno.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "Ndos.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "Nocho.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "Ncuatro.jpg",
          data: "",
        },
        {
          nombre: "",
          img: "Ntres.jpg",
          data: "",
        },      
      ],
    };
  },
};
</script>

<style>
</style>