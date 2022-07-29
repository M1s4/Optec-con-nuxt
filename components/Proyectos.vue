<template>
  <v-container fluid class="ma-0 pa-0" color="white">
    <v-card elevation="0" class="pt-3 px-3 rounded-0" color="white" light>
      <v-card elevation="0" class="rounded-0" light>
        <p class="cyan--text font-weight-bold text-caption">
          <v-icon left color="cyan">mdi-minus</v-icon>
          PROYECTOS RECIENTES
        </p>
        <p class="font-weight-black text-h5 pr-15">
          Nuestros Ultimos Proyectos
        </p>
      </v-card>
      <v-card elevation="0">
        <v-carousel
          height="auto"
          class="pb-13 custom"
          cycle
          interval="10000"
          :show-arrows="false"
          delimiter-icon="mdi-minus"
          hide-delimiter-background
        >
          <v-carousel-item v-for="(item, i) in proyectos" :key="i">
            <v-card
              class="mx-auto"
              max-width="400"
              light
              elevation="2"
              outlined
            >
              <v-img
                class="white--text align-end rounded-0"
                height="200px"
                :src="require(`../static/images/${item.srcImg}`)"
                gradient="to bottom, rgba(21,22,24,.2), rgba(21,22,24.1)"
              >
                <v-card-title class="text-subtitle-1 font-weight-black">{{
                  item.nombre
                }}</v-card-title>
                <v-card-subtitle class="text-caption">
                  {{ item.ciudad }}
                </v-card-subtitle>
              </v-img>

              <v-card-text class="text-body-1">
                {{ item.data }}
              </v-card-text>

              <v-card-actions>
                <v-btn
                  color="#09AEB8"
                  text
                  class="text-lowercase text-caption"
                  :to="item.url"
                >
                  Seguir leyendo <v-icon small right>mdi-skip-next</v-icon>
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-carousel-item>
        </v-carousel>
      </v-card>
    </v-card>
  </v-container>
</template>

<script lang="ts">
export default {
  data() {
    return {
      proyectos: [
        {
          nombre: "Mantenimiento preventivo a Minisplits.",
          ciudad: "Puerto Vallarta, Jalisco",
          srcImg: "tres.jpg",
          data: "Mantenimiento preventivo a Minisplits. Costo de servicio de 2 equipos en adelante $450.00 c/u. Presupuesto y visita técnica sin compromiso.",
          url: "/proyectos/minisplitmant",
        },
        {
          nombre: "Mantenimiento correctivo a Chiller",
          ciudad: "Puerto Vallarta, Jalisco",
          srcImg: "Nocho.jpg",
          data: "Mantenimiento correctivo a Chiller, cambio de sensor de flujo de agua, cambio de válvulas eliminadoras de aire, purga de sistema, actualización de software.",
          url: "/proyectos/mantchiller",
        },
        {
          nombre: "Instalación de bomba presurizadora",
          ciudad: "Puerto Vallarta, Jalisco",
          srcImg: "bypass.jpg",
          data: "Instalación de bomba presurizadora, con bypass.",
          url: "/proyectos/bombainst",
        },
        {
          nombre:
            "Mantenimiento preventivo y predictivo a sistema de paneles solares",
          ciudad: "Puerto Vallarta, Jalisco",
          srcImg: "panelS.jpg",
          data: "Mantenimiento preventivo y predictivo a sistema de paneles solares",
          url: "/proyectos/panelinst",
        },
        {
          nombre: "Cambio de tanque Hidroneumatico.",
          ciudad: "Puerto Vallarta, Jalisco",
          srcImg: "Hidroneumatico.jpg",
          data: "Cambio de tanque Hidroneumatico, con membrana dañada de años y tanque corroído.",
          url: "/proyectos/hidrouneumatico",
        },
      ],
    };
  },
};
</script>

<style>
#carousel-example-generic a.carousel-control {
  height: 30px;
  width: 30px;
}
.custom .v-carousel__controls__item.v-btn {
  color: grey !important;
}

.custom .v-carousel__controls__item.v-btn.v-btn--active {
  color: #f58a1a !important;
}
</style>
