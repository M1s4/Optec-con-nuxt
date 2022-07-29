<template>
  <v-container fluid class="ma-0 pa-0 "  color="white">
    <v-card class="ma-0 pa-0 py-md-15 pt-8 px-3 rounded-0 " elevation="0" light>
       <p class="font-weight-black text-h5 pr-15 pl-md-15">
        ¿Cuando dar mantenimiento a tu aire acondicionado?
      </p>
    <v-card elevation="0" class="pa-md-3 pt-4 rounded-0 pt-md-5 d-md-flex mx-auto" light width="90vw" >
     
      <nuxt-img
              :src="(`/images/tip.jpg`)"
              sizes="sm:60vw md:30vw lg:30vw"
              loading="lazy"
              min-height="150px"                
              class="mb-3"             
              quality="100"
              fit="cover"
              format="webp"  
            /> 
      <v-card elevation="0" light class="rounded-0 pr-md-15 pl-md-5 pt-md-3 ma-0">
        <p class="grey--text text-body-1 mr-md-15">
        Si un aire acondicionado no recibe un buen cuidado o un correcto
        mantenimiento, su tiempo de vida se reduce drásticamente ya que cuentan
        con piezas muy delicadas que precisan de recambios cada cierto tiempo,
        además de una limpieza periódica que ayude a evitar posibles creaciones
        de plagas bacterianas y de hongos en su interior, con la consecuente
        contaminación del aire de nuestros hogares y oficinas, provocando
        problemas de salubridad.
      </p>
      <div>
        <p class="font-weight-bold text-subtitle-1 pr-10">
          servicios que se ofrecen en el mantenimiento preventivo :
        </p>
        <div class="py-4 py-md-1">
          <p
            v-for="(item, i) in servicios"
            :key="i"
            text
            elevation="0"
            class="grey--text text-subtitle-2 ma-0 pa-0 mb-5"
          >
            <nuxt-img
              :src="(`/images/icons/${item.icon}`)"
              sizes="sm:100vw md:50vw lg:100vw"
              loading="lazy"
              width="15"
              class="mr-4"
              height="15"
              quality="80"
              fit="cover"
              format="webp"  
            />           
            {{ item.nombre }}
          </p>
        </div>
      </div>
      </v-card> 
      
    </v-card>
    </v-card>
    
  </v-container>
</template>

<script lang="ts">
export default {
  data() {
    return {
      servicios: [
        {
          nombre: "Mantenimiento de la unidad exterior",
          icon: "sliderDos1.svg",
        },
        {
          nombre: "Limpieza general de la unidad interior",
          icon: "sliderDos2.svg",
        },
        {
          nombre: "Limpieza del desagüe del split",
          icon: "sliderDos3.svg",
        },
      ],
    };
  },
};
</script>

<style>
</style>