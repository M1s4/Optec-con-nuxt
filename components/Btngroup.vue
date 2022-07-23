<template>
   <v-container fluid class="ma-0 pa-0">
     <v-speed-dial
      v-model="fab"
      :top="top"
      :bottom="bottom"
      :right="right"
      :left="left"
      :direction="direction"
      :open-on-hover="hover"
      :transition="transition"
      fixed 
    >
      <template v-slot:activator>
        <v-btn
          v-model="fab"
          color="blue darken-2"
          dark
          fab
          
        >
          <v-icon v-if="fab">
            mdi-close
          </v-icon>
          <v-icon v-else>
            mdi-message-reply-text
          </v-icon>
        </v-btn>
      </template>
     
      <v-btn
        fab
        dark
        small
        color="#4267B2"
        href="https://www.facebook.com/optecmantenimiento"
        target="_blank"
      >
        <v-icon>mdi-facebook</v-icon>
      </v-btn>
       <v-btn
        fab
        dark
        small
        color="#25D366"
        target="_blank"
        href="https://api.whatsapp.com/send?phone=3221884814&text=Hola!%20">      
        <v-icon>mdi-whatsapp</v-icon>
      </v-btn>
      <v-btn
        fab
        dark
        small
        color="#c71610"
        href="mailto:ing.davidjuarezc@gmail.com?Subject=Correo%20para%20informacion%20sobre%20Desarrollador%20FullStack"
      >
        <v-icon>mdi-gmail</v-icon>
      </v-btn>
    </v-speed-dial>
   </v-container>
</template>

<script lang="ts">
export default {
    data: () => ({
      direction: 'top',
      fab: false,
      fling: false,
      hover: false,
      tabs: null,
      top: false,
      right: true,
      bottom: true,
      left: false,
      transition: 'slide-y-reverse-transition',
    }),

}
</script>

<style>

</style>