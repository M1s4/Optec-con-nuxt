<template>
  <v-container fluid class="ma-0 pa-0">
    <v-card
      class="rounded-0 grey--text px-5 pt-10"
      color="#1D1C1D"
      max-width="100%"
    >
      <div class="d-flex justify-space-between">
        <div>
          <p class="font-weight-black white--text text-subtitle-2">
            Informacion de contacto
          </p>
          <div>
            <p class="text-caption mb-1">
              Puerto Vallarta, Jalisco Mexico
            </p>
            <p class="text-caption mb-1">
              Bahia de banderas, Nayarit
            </p>
            <p class="text-caption mb-1">(32) 1807041</p>
            <p class="text-caption mb-1">
              correo@hotmail.com
            </p>
          </div>
        </div>
        <div class="white--text text-center">
          <p class="font-weight-black white--text text-subtitle-2 ">Menu</p>
          <div class="d-flex flex-column justify-start">
            <v-btn class=" text-caption grey--text" text small @click="$vuetify.goTo('#inicio')"
              >Inicio</v-btn
            >
            <v-btn class=" text-caption grey--text" text small @click="$vuetify.goTo('#nosotros')"
              >Nosotros</v-btn
            >
            <v-btn class=" text-caption grey--text" text small @click="$vuetify.goTo('#servicios')"
              >Servicios</v-btn
            >
            <v-btn class=" text-caption grey--text" text small @click="$vuetify.goTo('#contacto')"
              >Contacto</v-btn
            >
          </div>
        </div>
      </div>
      <div class="d-flex justify-center flex-column mt-5">
        <v-card color="transparent" class="mx-auto my-5" elevation="0">
           <v-btn width="150" color="transparent" elevation="0" large class="mx-auto" text>
            <nuxt-img           
              loading="lazy"   
              width="140" :src="(`/images/icons/OPTECop2.svg`)"
              quality="80" 
              aspect-ratio="1.4"
              sizes="sm:180px md:50vw lg:100vw"               
              format="webp"              
             /> 
        </v-btn>
        <div class="mx-auto text-center mt-2">
          <v-btn icon small class="mx-2" href="https://api.whatsapp.com/send?phone=3221807041&text=Hola!%20" target="_blank">
            <v-icon color="white" icon small class=" pt-7">mdi-whatsapp</v-icon>
          </v-btn>
          <v-btn icon small class="mx-2" target="_blank" href="https://www.facebook.com/optecmantenimiento">
            <v-icon color="white" icon small class=" pt-7">mdi-facebook</v-icon>
          </v-btn>
        </div>
        </v-card>        
        <v-card
          class="d-flex justify-space-between mt-3 px-4"
          color="transparent"
          elevation="0"
        >
          <div v-for="(item, i) in bancos" :key="i">
            <nuxt-img
              :src="(`/images/icons/${item.src}`)"
              :width="item.alto"
              :height="item.ancho"
              alt=""
              class=""
            />
          </div>
        </v-card>
        <p class="text-caption grey--text text-center pt-2">
          © 2022 Todos los derechos recervados
        </p>
      </div>
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
          alto:"50",
          ancho:"30",
          nombre: "",
        },
        {
          src: "banco-santander-logo.svg",
          alto:"80",
          ancho:"30",
          nombre: "",
        },
        {
          src: "mastercard.svg",
         alto:"50",
          ancho:"30",
          nombre: "",
        },
        {
          src: "visa-svg.svg",
          alto:"50",
          ancho:"30",
          nombre: "",
        },
      ],
    };
  },
};
</script>