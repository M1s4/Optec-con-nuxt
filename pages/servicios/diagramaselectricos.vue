<template>
  <v-container fluid class="ma-0 pa-0">
    <v-container fluid class="ma-0 pa-0">
      <BtnBack />

      <v-card width="100%" color="red" height="130" class="text-center">
        <v-img
          class="white--text align-center rounded-0"
          height="100%"
          :src="require(`@/assets/images/controlsAC.jpg`)"
          gradient="to bottom, rgba(21,22,24,.2), rgba(21,22,24.1)"
        >
          <v-card class="text-center" color="transparent" elevation="0">
            <v-card-subtitle
              class="text-caption pb-0 mb-0 font-weight-black white--text"
            >
              Servicios</v-card-subtitle
            >
            <v-card-subtitle
              class="text-subtitle-2 pa-0 pt-2 white--text font-weight-normal"
            >
              Diagramas electricos
            </v-card-subtitle>
          </v-card>
        </v-img>
      </v-card>

      <v-card
        width="100%"
        light
        elevation="0"
        class="text-center rounded-0 pt-13 pb-5 px-5"
      >
        <p class="font-weight-black text-h6 text-md-h5">
          Servicio de diagramas y planos electricos
        </p>
        <v-img
          class="white--text align-end rounded-0"
          height="190px"
          :src="require(`@/assets/images/diagramas.jpg`)"
        >
        </v-img>
        <p class="pt-8 grey--text text-body-1 text-left font-weight-normal">
          Realizamos levantamiento de la distribución de cargas, arreglo de
          subestaciones, distribución de sistemas de puesta a tierra,
          actualización de diagramas unifilares, alimentadores, etc.
        </p>
        <p class="grey--text text-body-1 text-left font-weight-normal">
          Es muy importante señalar que los planos de una instalación eléctrica
          deben estar actualizados y estar siempre a la mano para consultas
          técnicas y para saber la distribución y tipo de cargas conectadas.
          Desconocer las tensiones de funcionamiento de los equipos, sobre
          cargar un circuito o exceder las capacidades de operación, puede
          generar daños severos a la instalación y exponer a los usuarios a
          graves riesgos, tales como, quemaduras o descargas eléctricas que
          pueden llegar a ser mortales.
        </p>
      </v-card>

      <v-card class="py-8 rounded-0 px-3" light elevation="0">
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