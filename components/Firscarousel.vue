<template>
  <v-container fluid  class="pa-0 ma-0" style="height:550px;">
    <v-carousel
      width="100%"  
      height="550"
      hide-delimiters
      :show-arrows="false"
      class="ma-0 pa-0"
      interval="15000"
    >
      <v-carousel-item v-for="(item, i) in items" :key="i">
        <v-sheet color="grey" >
          <nuxt-img src="/images/uno.jpg" sizes="sm:100vw md:50vw lg:400px" />
          
        </v-sheet>
      </v-carousel-item>
    </v-carousel>
     <v-card absolute width="320" height="370" id="vCard" class="rounded-0 grey--text">
               <div class="py-10 px-8">
                <p class="mb-0 text-caption" style="color:#09AEB8;">
                  Comprometidos con servicios de primera calidad
                </p>
                <p class="font-weight-black text-h4 white--text">
                  Servicios de Instalacion, Proyectos & Mantenimiento
                </p>
                <v-btn color="#FFD763" class=" black--text text-caption font-weight-bold mt-3 py-7 px-5 rounded-0" href="https://api.whatsapp.com/send?phone=3221807041&text=Hola!%20" target="_blank">
                  obtenga su cotizacion gratis
                </v-btn>
               </div>
     </v-card>
  </v-container>
</template>

<script lang="ts">
export default {
  name: "FirstCarousel",
  data() {
    return {
      colors: [
        "indigo",
        "warning",
        "pink darken-2",
        "red lighten-1",
        "deep-purple accent-4",
      ],
        items: [
      {
        title: "Tienda en linea",
        precio: "9000",
        text: `It's New Release Friday`,
        horario: "16:20",
        horario2: "20:16",
        subtext: "Newly released songs. Updated daily.",
        img: "uno.jpg",
      },
      {
        title: "Web con blog",
        text: "Greatest Rock Hits",
        subtext: "Lose yourself in rock tunes.",
        precio: "9000",
        horario2: "20:16",
        img: "dos.jpg",
      },
      {
        title: "Web para empresa",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        precio: "9000",
        horario2: "20:16",
        img: "Nsiete.jpg",
      },
      {
        title: "Web para empresa",
        text: "Ambient Bass",
        subtext: "Chill beats to mellow you out.",
        precio: "9000",
        horario2: "20:16",
        img: "seis.jpg",
      },         
    ],
      slides: ["First", "Second", "Third", "Fourth", "Fifth"],
    };
  },
};
</script>

<style>
  #vCard{
    background-color:rgba(29, 28, 29, 0.81) !important;
    margin-top:-420px;
    margin-bottom:70px;
  }
</style>