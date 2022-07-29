<template lang="html">
  <v-container fluid class="ma-0 pa-0" color="white">   

    <v-container fluid class="ma-0 pa-0">
      <BtnBack/>

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
              Instalacion AC
            </v-card-subtitle>
          </v-card>
        </v-img>
      </v-card>

      <v-card
        max-width="100%"        
        elevation="0"
        class="text-center pt-13 pb-5 px-5 rounded-0"
        light
        
      >
        <p class="font-weight-black text-h6 text-md-h5">
          Servicio de Instalacion de Aire Acondicionado
        </p>
        <nuxt-img              
             sizes="sm:43vw md:50vw lg:100vw" 
             width="70vh"
             height="178px"             
             loading="lazy"      
             quality="80" 
             class="white--text align-end rounded-0"
             :src="(`/images/reemplazodos.jpg`)"
             format="webp" 
             />            
        <p class="pt-8 grey--text text-body-1 text-left font-weight-normal">
          En OPTEC contamos con personal capacitado para hacer una instalación profesional de equipo de aire acondicionado doméstico e industrial.
        </p>
        <p class=" grey--text text-body-1 text-left font-weight-normal">
          Garantizamos a nuestros clientes la funcionalidad total de sus aparatos de aire acondicionado, así como excelentes resultados en los trabajos que realizamos de plomería y electricidad. Ofrecemos honestidad, trato esmerado y respetuoso, además de los precios más accesibles del mercado.
        </p>
      </v-card>

      <v-card width="100%" light elevation="0" class="px-5 pt-10 rounded-0">
        <p class="font-weight-black text-h6 text-md-h5 black--text">
          Problemas comunes en aires acondicionados
        </p>
        <nuxt-img
                  sizes="md:50vw lg:100vw"
                  width="333"
                  loading="lazy"                  
                  height="170px"
                  :src="(`/images/tres.jpg`)"
                  quality="80"
                  fit="cover"
                  class="white--text align-end rounded-0"
                />
 
        <v-card class="pt-6" color="transparent" elevation="0" width="100%">
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

      <v-card class="px-5 pt-5 pb-10 rounded-0" elevation="0" light>
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