<template>
   <v-container fluid class="ma-0 pa-0" >

    <v-card elevation="0" class="pa-3 rounded-0 pt-9" light>
        <p class="cyan--text font-weight-bold text-caption">
            <v-icon left color="cyan">mdi-minus</v-icon>
              NUESTROS SERVICIOS
        </p>
        <p class="font-weight-black text-h5 pr-15">Brindamos una gama completa de servicios para su hogar.</p>
        <p class="grey--text text-body-1">
            Si un aire acondicionado no recibe un buen cuidado o un correcto mantenimiento,
            su tiempo de vida se reduce drásticamente ya que cuentan con piezas muy delicadas
            que precisan de recambios cada cierto tiempo.
        </p>
    </v-card> 

    <v-carousel  height="auto" cycle interval="10000" hide-delimiters light >
      <v-carousel-item
        v-for="(item,i) in servicios" 
        :key="i"      
        
        >
        <v-card class="d-flex pa-3 rounded-0" elevation="0" light >
          <img 
          width="30" 
          height="30"
          :src="require(`../assets/images/icons/${item.icon}`)"
          >

          <img/>
          <div class="pl-5">
            <p class="font-weight-black text-subtitle-1">{{item.nombre}}</p>
            <p class="grey--text text-subtitle-2">{{item.datos}}</p>

            <v-btn text :to="item.ruta" class="px-0 grey--text text-caption font-weight-bold">leer mas <v-icon right>mdi-chevron-right</v-icon></v-btn>
          </div>
        </v-card>       
      </v-carousel-item>
    </v-carousel>

    <v-card class="d-flex justify-center pt-3 rounded-0" elevation="0" light>
      <v-btn 
      color="#FFD763" 
      class="font-weight-normal rounded-0 py-6 text-lowercase text--grey-darken-4" 
      width="90%"
      href="https://api.whatsapp.com/send?phone=3221807041&text=Hola!%20"
      target="_blank"
      >
        <v-icon left>
          mdi-cellphone-text
        </v-icon>
        pedir cotizacion
        </v-btn>
     </v-card>

   </v-container>
</template>

<script lang="ts">
  export default {
    data () {
      return {       
        servicios: [
            {
                nombre:'A/C Instalacion',
                datos:'En OPTEC contamos con personal capacitado para hacer una instalación profesional de equipo de aire acondicionado doméstico e industrial.',
                icon:'AC.svg',
                 ruta: "/servicios/acinstalacion",
            },            
             {
                nombre:'Instalaciones electricas en baja tension',
                datos:'contamos con un equipo altamente cualificado para realizar las instalaciones eléctricas de baja tensión, así como las líneas de media tensión de un modo totalmente seguro y económico.',
                icon:'bajatension.svg',
                ruta: "/servicios/bajatencion",
            },
            {
                nombre:'AC Reparacion y mantenimiento',
                datos:'En OPTEC contamos con las herramientas y refacciones necesarias para realizas cualquier tipo de repararción a equipos domesticos e industriales. Realizamos los procedimientos adecuados y respetamos la infraestructura del edificio',
                icon:'mainenceAC.svg',
                ruta: "/servicios/acmantenimiento",
            },
            {
                nombre:'Diagramas electricos / Planos Electricos',
                datos:'Realizamos levantamiento de la distribución de cargas, arreglo de subestaciones, distribución de sistemas de puesta a tierra, actualización de diagramas unifilares, alimentadores, etc.',
                icon:'plan.png',
                ruta: "/servicios/diagramaselectricos",
            }
        ],
      }
    },
  }
</script>

<style>
  #carousel-example-generic a.carousel-control {
  height: 30px;
  width: 30px;
  }
</style>
