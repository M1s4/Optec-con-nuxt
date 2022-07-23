<template>
  <v-container fluid class="ma-0 pa-0 " color="white">
   <v-card elevation="0" class="pa-3 rounded-0 py-9" light>        
        <p class="font-weight-black text-h5 pr-15">¿Cuando dar mantenimiento a tu aire acondicionado?</p>
        <p class="grey--text text-body-1">
            Si un aire acondicionado no recibe un buen cuidado o un correcto mantenimiento,
            su tiempo de vida se reduce drásticamente ya que cuentan con piezas muy delicadas
            que precisan de recambios cada cierto tiempo, además de una limpieza periódica que
            ayude a evitar posibles creaciones de plagas bacterianas y de hongos en su interior,
            con la consecuente contaminación del aire de nuestros hogares y oficinas, provocando
            problemas de salubridad.
        </p>
        <div>
            <p class="font-weight-bold text-subtitle-1 pr-10">
                servicios que se ofrecen en el mantenimiento preventivo :
            </p>
            <div class="">
              <p v-for="(item,i) in servicios" :key="i" text elevation="0" class="grey--text text-subtitle-2 ma-0 pa-0 mb-5">
                    <img 
                width="15"
                class="mr-4" 
                height="15"
                :src="require(`@/assets/images/icons/${item.icon}`)"
                >
                <img/>
               {{item.nombre}}
            </p>
            </div>            
        </div>
    </v-card> 
  </v-container>
</template>

<script lang="ts">
export default {

data(){
    return{
        servicios: [
            {
                nombre:'Mantenimiento de la unidad exterior',
                icon:'sliderDos1.svg'
            },
            {
                nombre:'Limpieza general de la unidad interior',
                icon:'sliderDos2.svg'
            },
            {
                nombre:'Limpieza del desagüe del split',
                icon:'sliderDos3.svg'
            }
        ]
    }
}
}
</script>

<style>

</style>