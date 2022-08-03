<template>
  <v-container fluid class="ma-0 pa-0">
    <v-container fluid class="ma-0 pa-0">
      <BtnBack />

      <v-card width="100%" color="red" height="130" class="text-center">
        <v-img
          class="white--text align-center rounded-0"
          height="100%"
          :src="`/images/controlsAC.jpg`"
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

      <v-card class="ma-0 pa-0 rounded-0" elevation="0" light max-width="100vw">
        <v-card
          class="ma-0 pa-0 rounded-0 mx-auto d-md-flex"
          elevation="0"
          light
          max-width="85vw"
        >
          <v-card
            class="ma-0 pa-0 rounded-0"
            elevation="0"
            color="red"
            max-width="60vw"
          >
            <v-card
              width="100%"
              light
              elevation="0"
              class="text-center text-md-start rounded-0 pt-13 pb-5 px-5"
            >
              <p class="font-weight-black text-h6 text-md-h5">
                Servicio de diagramas y planos electricos
              </p>
              <nuxt-img
                loading="lazy"
                width="333px"
                :src="`/images/diagramas.jpg`"
                quality="80"
                aspect-ratio="1.4"
                sizes="sm:180px md:50vw lg:100vw"
                format="webp"
                height="190px"
                class="white--text align-end rounded-0"
              />
              <p
                class="pt-8 grey--text text-body-1 text-left font-weight-normal"
              >
                Realizamos levantamiento de la distribución de cargas, arreglo
                de subestaciones, distribución de sistemas de puesta a tierra,
                actualización de diagramas unifilares, alimentadores, etc.
              </p>
              <p class="grey--text text-body-1 text-left font-weight-normal">
                Es muy importante señalar que los planos de una instalación
                eléctrica deben estar actualizados y estar siempre a la mano
                para consultas técnicas y para saber la distribución y tipo de
                cargas conectadas. Desconocer las tensiones de funcionamiento de
                los equipos, sobre cargar un circuito o exceder las capacidades
                de operación, puede generar daños severos a la instalación y
                exponer a los usuarios a graves riesgos, tales como, quemaduras
                o descargas eléctricas que pueden llegar a ser mortales.
              </p>
            </v-card>

            <v-card class="pt-3 pb-7 rounded-0 px-3" light elevation="0">
              <v-btn
                color="#FFD763"
                class="
                  font-weight-normal
                  rounded-0
                  py-6
                  text-lowercase text--grey-darken-4
                "
                min-width="350"
                max-width="350px"
                href="https://api.whatsapp.com/send?phone=3221884814&text=Hola!%20"
                target="_blank"
              >
                <v-icon left> mdi-cellphone-text </v-icon>
                pedir cotizacion
              </v-btn>
            </v-card>
          </v-card>
          <v-card
            class="ma-0 pa-0 rounded-0 d-none d-md-inline"
            light
            elevation="0"
            max-width="20vw"
          >
            <v-card class="pt-md-15" elevation="0">
              <p class="font-weight-black text-md-subtitle-1">
                Nuestros Servicios
              </p>
              <v-card class="ma-0 pa-0 rounded-0 pt-5" elevation="0">
                <p class="text-md-body-2 font-md-weight-medium">
                  A/C INSTALACION
                </p>
                <p class="text-md-body-2 font-md-weight-medium">
                  Mantenimiento y reparacion
                </p>
                <p class="text-md-body-2 font-md-weight-medium">Reemplazo</p>
                <p class="text-md-body-2 font-md-weight-medium">
                  Reemplazo y reparacion
                </p>
              </v-card>

              <v-card class="ma-0 pa-0 rounded-0" elevation="0">
                <p
                  class="
                    font-weight-black
                    text-md-subtitle-1 text-center
                    pt-md-9
                  "
                >
                  ¿Cree que su unidad de aire acondicionado requiere un servicio
                  de emergencia?
                </p>
                <v-card
                  class="
                    ma-0
                    pa-4
                    rounded-0
                    font-weight-black
                    white--text
                    text-center text-body-2
                  "
                  elevation="0"
                  color="#EA0A3B"
                  max-width="20vw"
                >
                  Agenda cita de emergencia (322) 1807041
                </v-card>
              </v-card>
            </v-card>
          </v-card>
        </v-card>
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