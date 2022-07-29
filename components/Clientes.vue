<template>
  <v-container fluid class="text-center pa-0 ma-0">
    <v-card light class="rounded-0 pt-9 px-3 pb-15">
        <v-card elevation="0" class=" rounded-0" light>
      <p class="font-weight-black text-h6 text-center" style="color: #09aeb8">
        Damos servicio, reparamos e instalamos todas las marcas
      </p>
      <p class="grey--text text-body-1">
        Ofrecemos reparación, mantenimiento e instalación de las principales
        marcas de equipos de enfriamiento de aire
      </p>
        </v-card>
        <v-slide-group v-model="model" class="px-7 py-5" light>
        <v-slide-item
            v-for="(item, i) in marcas"
            :key="i"                                    
            >
            <v-card
            class=" rounded-0"            
            elevation="0"
            >
            <nuxt-img           
             loading="lazy"              
             :width="item.width"
             :height="item.height"
             :src="(`/images/${item.img}`)"
             quality="80" 
             format="webp"  
             class="px-7"            
             />      
            </v-card>
        </v-slide-item>
        </v-slide-group>
    </v-card>
   
  </v-container>
</template>

<script lang="ts">
export default {
  data() {
    return {
      marcas: [
     
        {
          nombre: "",
          with:"35px",
          height:"35px",
          img: "logo-lg.svg",
        },
        {
          nombre: "",
          with:"33px",
          height:"33px",
          img: "samsung.svg",
        },
        {
          nombre: "",
          with:"30px",
          height:"30px",
          img: "toshiba.svg",
        },
        {
          nombre: "",
          with:"60px",
          height:"40px",
          img: "general-electric.svg",
        },
      ],
      model: null,
    };
  },
};
</script>