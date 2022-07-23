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
        <v-slide-group v-model="model" class="px-7 py-5" active-class="success" light>
        <v-slide-item
            v-for="(item, i) in marcas"
            :key="i"
            v-slot="{  toggle }" 
            >
            <v-card
            class="mr-13 rounded-0"
            height="40"
            width="75"
            elevation="0"
            @click="toggle"
            >
            <img
                width="100%"
                height="100%"
                :src="require(`../assets/images/${item.img}`)"
            />
            <img />
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
          img: "logo-lg.svg",
        },
        {
          nombre: "",
          img: "samsung.svg",
        },
        {
          nombre: "",
          img: "toshiba.svg",
        },
        {
          nombre: "",
          img: "GG.png",
        },
      ],
      model: null,
    };
  },
};
</script>