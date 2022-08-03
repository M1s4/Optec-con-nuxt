<template>
  <v-container fluid class="ma-0 pa-0">
    <v-card elevation="0" class="pt-10 pb-7 rounded-0 px-3 px-md-0" light>
      <v-card
        class="ma-0 pa-0 rounded-0 d-md-flex justify-md-center mx-md-auto"
        light
        elevation="0"
        max-width="85vw"
      >
        <v-card class="ma-0 pa-0 rounded-0" elevation="0" light>
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

          <p class="grey--text text-body-1 pr-md-15">
            En <strong>OPTEC</strong> somos una empresa que contamos con un
            equipo de Ingenieros experimentados, calificados y confiables que
            brinda soluciones integrales de ingenieria, proyectos de obra
            eléctrica, mantenimiento industrial y residencial para propiedades
            residenciales y comerciales.
          </p>
        </v-card>

        <v-row justify="space-around">
          <v-card width="100%" elevation="0">
            <v-slide-group class="pa-4">
              <v-slide-item
                v-for="(item, i) in nosotros"
                :key="i"
                v-slot="{ toggle }"
                class="px-2"
              >
                <v-card
                  class="pa-0 rounded-0"
                  min-height="200"
                  max-height="400"
                  min-width="180"
                  max-width="100"
                  @click="toggle"
                >
                  <nuxt-img
                    sizes="sm:45vw md:80vw lg:30vw"
                    loading="lazy"
                    width="100%"
                    :src="`/images/${item.img}`"
                    quality="80"
                    fit="cover"
                    class="pa-0 ma-0"
                    format="webp"
                  />
                </v-card>
              </v-slide-item>
            </v-slide-group>
          </v-card>
        </v-row>
      </v-card>

      <v-card
        class="d-flex justify-center justify-md-start pl-md-10 pt-3 rounded-0 "
        elevation="0"
        light
       >
        <v-btn
          color="#FFD763"
          class="
            mt-md-n16
            font-weight-normal
            rounded-0
            py-6
            ml-md-10
            text-lowercase text--grey-darken-4
          "
          width="90%"
          href="https://api.whatsapp.com/send?phone=3221807041&text=Hola!%20"
          target="_blank"
          max-width="35vw"
          min-width="333px"
          
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
      ],
    };
  },
};
</script>

<style>
</style>