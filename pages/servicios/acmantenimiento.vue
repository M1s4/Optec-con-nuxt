<template>
  <v-container fluid class="ma-0 pa-0">
    <BtnBack/>
    <v-container fluid class="ma-0 pa-0 ">

      <v-card width="100%" color="red" height="130" class="text-center">
        <v-img
          class="white--text align-center rounded-0"
          height="100%"
          :src="require(`../../assets/images/controlsAC.jpg`)"
          gradient="to bottom, rgba(21,22,24,.2), rgba(21,22,24.1)"
        >
          <v-card class="text-center" color="transparent" elevation="0">
            <v-card-subtitle
              class="text-caption pb-0 mb-0 font-weight-black white--text"
            >
              Servicios</v-card-subtitle
            >
            <v-card-subtitle class="text-subtitle-2 pa-0 pt-2 white--text font-weight-normal">
              AC reparacion y mantenimiento
            </v-card-subtitle>
          </v-card>
        </v-img>
      </v-card>

      <v-card
        width="100%"
        light
        elevation="0"
        class="text-center rounded-0 pt-13 px-5 pb-4"
      >
        <p class="font-weight-black text-h6 text-md-h5">
          Servicio de reparacion y mantenimiento a aires acondicionas
        </p>
        <v-img
          class="white--text align-end rounded-0"
          height="190px"
          :src="require(`../../assets/images/cuatro.jpg`)"
        >
        </v-img>
        <p class="pt-8 grey--text text-body-1 text-left font-weight-normal">
          En OPTEC contamos con las herramientas y refacciones necesarias para
          realizas cualquier tipo de repararción a equipos domesticos e industriales.
          Realizamos los procedimientos adecuados y respetamos la infraestructura del edificio
        </p>
      </v-card>

      <v-card width="100%" light elevation="0" class="px-5 pt-10 rounded-0">
        <p class="font-weight-black text-h6 text-md-h5 black--text">
          Problemas comunes en aires acondicionados
        </p>
        <v-img
          class="white--text align-end rounded-0"
          height="160px"
          :src="require(`../../assets/images/tres.jpg`)"
        >
        </v-img>
        <v-card class="mt-6" color="transparent" elevation="0" width="100%">
          <div class="d-flex pt-4">
            <v-icon color="#EA0A3B" small left>mdi-alert-circle-check</v-icon>
            <p class="mb-0 text-body-2 grey--text">
              El aire acondicionado no se enciende.
            </p>
          </div>

          <div class="d-flex pt-4">
            <v-icon color="#EA0A3B" small left>mdi-alert-circle-check</v-icon>
            <p class="mb-0 text-body-2 grey--text">
              Se producen ruidos extraños o vibraciones al arrancar o durante el
              funcionamiento.
            </p>
          </div>

          <div class="d-flex pt-4">
            <v-icon color="#EA0A3B" small left>mdi-alert-circle-check</v-icon>
            <p class="mb-0 text-body-2 grey--text">
              El aire caliente sale de los registros de suministro.
            </p>
          </div>

          <div class="d-flex pt-4">
            <v-icon color="#EA0A3B" small left>mdi-alert-circle-check</v-icon>
            <p class="mb-0 text-body-2 grey--text">
              La unidad zumba, pero el ventilador no se enciende.
            </p>
          </div>

          <div class="d-flex pt-4">
            <v-icon color="#EA0A3B" small left>mdi-alert-circle-check</v-icon>
            <p class="mb-0 text-body-2 grey--text">
              El ventilador funciona, pero el compresor no funciona.
            </p>
          </div>

          <div class="d-flex pt-4">
            <v-icon color="#EA0A3B" small left>mdi-alert-circle-check</v-icon>
            <p class="mb-0 text-body-2 grey--text">
              El agua se acumula alrededor del acondicionador de aire
            </p>
          </div>
        </v-card>
      </v-card>

      <v-card class="py-10 px-3 pt-10 rounded-0" elevation="0" light>
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

    </v-container>
  </v-container>
</template>

<script lang="ts">
import BtnBack from "../../components/BtnBack.vue";
export default {
  components: {
    BtnBack,
  },
};
</script>

<style>
</style>