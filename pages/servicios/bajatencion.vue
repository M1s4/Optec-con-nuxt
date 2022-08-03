<template>
  <v-container fluid class="ma-0 pa-0">
    <BtnBack />
    <v-card elevation="0" class="ma-0 pa-0 mx-md-auto" max-width="100vw" light>
      <v-card width="100%" height="130" class="text-center">
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
              Instalaciones electricas en baja tension
            </v-card-subtitle>
          </v-card>
        </v-img>
      </v-card>

      <v-card class="ma-0 pa-0 rounded-0 d-md-flex mx-auto" color="red" elevation="0" min-width="" max-width="85vw" >

        <v-card elevation="0" class="ma-0 pa-0 mx-auto pr-md-8" max-width="100%" width="100vw" >
          <v-card
            width="100%"
            light
            elevation="0"
            class="text-center text-md-start pt-13 rounded-0"
          >
            <p class="font-weight-black text-h6 text-md-h5">
              Instalaciones electricas baja tension
            </p>
            <v-img
              class="white--text align-end rounded-0"
              height="190px"
              :src="require(`../../assets/images/Nsiete.jpg`)"
            >
            </v-img>
            <p class="pt-8 grey--text text-body-1 text-md-subtitle-1 text-left font-weight-normal">
              contamos con un equipo altamente cualificado para realizar las
              instalaciones eléctricas de baja tensión, así como las líneas de
              media tensión de un modo totalmente seguro y económico.
            </p>

            <v-card
              class="mt-6 text-left px-2"
              color="transparent"
              elevation="0"
              width="100%"
            >
              <p class="font-weight-bold">Te podemos ayudar con :</p>
              <div class="d-flex pt-2">
                <v-icon class="pr-3" small left>mdi-check-bold</v-icon>
                <p class="mb-0 text-body-2 text-md-subtitle-1 grey--text">Tierras fisicas.</p>
              </div>

              <div class="d-flex pt-4">
                <v-icon class="pr-3" small left>mdi-check-bold</v-icon>
                <p class="mb-0 text-body-2 text-md-subtitle-1  grey--text">
                  Montajes de subestaciones eléctricas de media y baja tensión,
                  transformadores y tableros generales de distribución.
                </p>
              </div>

              <div class="d-flex pt-4">
                <v-icon class="pr-3" small left>mdi-check-bold</v-icon>
                <p class="mb-0 text-body-2 text-md-subtitle-1  grey--text">
                  Montajes de plantas de emergencia y tableros de transferencia
                </p>
              </div>

              <div class="d-flex pt-4">
                <v-icon class="pr-3" small left>mdi-check-bold</v-icon>
                <p class="mb-0 text-body-2 text-md-subtitle-1  grey--text">
                  Montajes de bancos de capacitores y filtros de armónicas.
                </p>
              </div>

              <div class="d-flex pt-4">
                <v-icon class="pr-3" small left>mdi-check-bold</v-icon>
                <p class="mb-0 text-body-2 text-md-subtitle-1  grey--text">
                  Montajes de circuitos de fuerza, alumbrado y contactos.
                </p>
              </div>

              <div class="d-flex pt-4">
                <v-icon class="pr-3" small left>mdi-check-bold</v-icon>
                <p class="mb-0 text-body-2 text-md-subtitle-1  grey--text">
                  Fabricación de tableros de fuerza.
                </p>
              </div>
              <div class="d-flex pt-4">
                <v-icon class="pr-3" small left>mdi-check-bold</v-icon>
                <p class="mb-0 text-body-2 text-md-subtitle-1  grey--text">
                  Montajes de sistemas de tierras físicas y pararrayos.
                </p>
              </div>
              <div class="d-flex pt-4">
                <v-icon class="pr-3" small left>mdi-check-bold</v-icon>
                <p class="mb-0 text-body-2 text-md-subtitle-1  grey--text">
                  Estudios de corto circuito y coordinación de protecciones y
                  flujos de potencia.
                </p>
              </div>
            </v-card>
          </v-card>

          <v-card class="px-5 px-md-0 py-12 rounded-0" elevation="0" light >
            <v-btn
              color="#FFD763"
              class="
                font-weight-normal
                rounded-0
                py-6
                text-lowercase text--grey-darken-4
              "
              width="100%"
              max-width="35vw"
              min-width="300"
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
                class="font-weight-black text-md-subtitle-1 text-center pt-md-9"
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