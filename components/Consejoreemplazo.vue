<template>
  <v-container fluid class="pa-0 ma-0">
    <v-card class="px-5 pt-10 pb-5 rounded-0" width="100%" elevation="0" light> 
      <p class=" mb-3 text-subtitle-2 font-weight-black text-center">
        ¿No sabes si reemplazar tu aire acondicionado?, Toma estos consejos en
        cuenta.
      </p>
      <v-img
        lazy-src="https://picsum.photos/id/11/10/6"
        max-height="150"
        max-width="550"
        width="100%"
        aspect-ratio="1.4"
        :src="require(`@/assets/images/reemplazodos.jpg`)"
        
      ></v-img>
      <v-card class="px-2 pt-8" elevation="0">
        <div class="d-flex" v-for="(item,i) in consejos" :key="i">
            <v-icon color="#EA0A3B" class="pr-4" left>mdi-{{item.icon}}</v-icon>
            <p class="text-body-2">
                {{item.data}}
            </p>
        </div>
      </v-card>
    </v-card>
  </v-container>
</template>

<script lang="ts">
export default {
    data (){
        return{
            consejos:[
                {
                    data:'Si su aire acondicionado tiene más de 10 años y le da problemas, puede ser en su mejor interés de considerar un reemplazo',
                    icon:'alert-circle-check'
                },
                {
                    data:'¿Es un nuevo sistema una mejor inversión a largo plazo?Nuestros Ingenieros pueden ayudarle a calcular el retorno de la inversión para determinar si una actualización es más beneficiosa que una reparación.',
                    icon:'alert-circle-check'
                },
                {
                    data:'Una unidad más eficiente consume menos electricidad y podría ahorrarle mucho en las facturas de energía.',
                    icon:'alert-circle-check'
                }
            ]
        }
    }
};
</script>

<style>
</style>