<template>
  <v-container fluid class="ma-0 pa-0">
    
     <firscarousel/>
     <servicios id="servicios"/>
     <mainencetip/>
     <proyectos id="proyectos"/>
     <consejoreemplazo/>
     <nosotros id="nosotros"/>
     <clientes/>
     <contacto id="contacto"/>

  </v-container>
</template>

<script>
import Btngroup from '../components/Btngroup.vue'
import Firscarousel from '../components/Firscarousel.vue'
export default {
  components: { Firscarousel, Btngroup },
  name: 'IndexPage'
}
</script>
