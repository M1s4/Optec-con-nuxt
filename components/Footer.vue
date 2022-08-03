<template>
  <v-container fluid class="ma-0 pa-0" color="#1D1C1D">
    <v-card class="ma-0 pa-0" color="#1D1C1D" elevation="0" max-width="100vw">
      <v-card
        class="pa-0 ma-0 rounded-0 grey--text px-5 px-md-0 pt-10 mx-md-auto d-md-flex justify-md-space-between "
        color="#1D1C1D"
        max-width="85vw"
        elevation="0"
      >
        <v-card class="d-flex justify-space-between pa-0 ma-0" elevation="0" max-width="90vw" width="53vw">
          <div>
            <p class="font-weight-black white--text text-subtitle-2 text-md-subtitle-1">
              Informacion de contacto
            </p>
            <div>
              <p class="text-caption mb-1 text-md-body-2">Puerto Vallarta, Jalisco Mexico</p>
              <p class="text-caption mb-1 text-md-body-2">Bahia de banderas, Nayarit</p>
              <p class="text-caption mb-1 text-md-body-2">(32) 1807041</p>
              <p class="text-caption mb-1 text-md-body-2">correo@hotmail.com</p>
            </div>
          </div>
          <div class="white--text text-center">
            <p class="font-weight-black white--text text-subtitle-2">Menu</p>
            <div class="d-flex flex-column flex-md-row justify-md-start  justify-start">
              <v-btn
                class="text-caption"
                text
                small
                @click="$vuetify.goTo('#inicio')"
                >Inicio</v-btn
              >
              <v-btn
                class="text-caption "
                text
                small
                @click="$vuetify.goTo('#nosotros')"
                >Nosotros</v-btn
              >
              <v-btn
                class="text-caption "
                text
                small
                @click="$vuetify.goTo('#servicios')"
                >Servicios</v-btn
              >
              <v-btn
                class="text-caption "
                text
                small
                @click="$vuetify.goTo('#contacto')"
                >Contacto</v-btn
              >
            </div>
          </div>
        </v-card>
        
        <v-card class="d-flex justify-center flex-column mt-5 mt-md-0 ma-0 pa-0 " elevation="0" >
          <v-card  class="mx-auto mt-5" elevation="0">
            <v-btn
              width="150"
              color="transparent"
              elevation="0"
              large
              class="mx-auto"
              text
            >
              <nuxt-img
                loading="lazy"
                width="140"
                :src="`/images/icons/OPTECop2.svg`"
                quality="80"
                aspect-ratio="1.4"
                sizes="sm:180px md:50vw lg:100vw"
                format="webp"
              />
            </v-btn>
            <div class="mx-auto text-center mt-2">
              <v-btn
                icon
                small
                class="mx-2"
                href="https://api.whatsapp.com/send?phone=3221807041&text=Hola!%20"
                target="_blank"
              >
                <v-icon color="white" icon small class="pt-7"
                  >mdi-whatsapp</v-icon
                >
              </v-btn>
              <v-btn
                icon
                small
                class="mx-2"
                target="_blank"
                href="https://www.facebook.com/optecmantenimiento"
              >
                <v-icon color="white" icon small class="pt-7"
                  >mdi-facebook</v-icon
                >
              </v-btn>
            </div>
          </v-card>
          <v-card
            class="d-flex justify-space-between mt-3 px-4"
            color="transparent"
            elevation="0"
          >
            <div v-for="(item, i) in bancos" :key="i" class="mx-md-2 mt-md-4">
              <nuxt-img
                :src="`/images/icons/${item.src}`"
                :width="item.alto"
                :height="item.ancho"
                alt=""
                class=""
              />
            </div>
          </v-card>
          
        </v-card>
        
      </v-card>
      <p class="text-caption grey--text text-center pt-2 mb-md-0 pb-md-2">
            © 2022 Todos los derechos recervados
          </p>
    </v-card>
  </v-container>
</template>

<script lang="ts">
export default {
  data() {
    return {
      bancos: [
        {
          src: "bbva-2019.svg",
          alto: "50",
          ancho: "30",
          nombre: "",
        },
        {
          src: "banco-santander-logo.svg",
          alto: "80",
          ancho: "30",
          nombre: "",
        },
        {
          src: "mastercard.svg",
          alto: "50",
          ancho: "30",
          nombre: "",
        },
        {
          src: "visa-svg.svg",
          alto: "50",
          ancho: "30",
          nombre: "",
        },
      ],
    };
  },
};
</script>