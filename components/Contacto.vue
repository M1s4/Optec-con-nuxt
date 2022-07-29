<template>
  <v-container fluid class="ma-0 pa-0">
    <v-card
      class="d-flex pa-0 ma-0 "
      outlined
      tile      
      height="auto"
      light
      color="white"
    >
      <transition name="fade">
        <v-card
          class="contentForm mt-10 ml-md-15 py-5 px-15"
          elevation="6"
          width="400px"
          v-if="show"
        >
          <v-form ref="form" class="Formulario pt-5" lazy-validation>
            <div class="font-weight-black text-h6 text-md-h5">
              INFORMACION DE CONTACTO
            </div>
            <div class="d-flex flex-column align- pb-5 pt-3 grey--text">
              <div class="pt-3 text-body-2 font-weight-bold">
                <v-icon class="pr-3" left small>mdi-phone</v-icon>
                322 188 48 14
              </div>

              <div class="pt-5 text-body-2 font-weight-bold">
                <v-icon class="pr-3" left small>mdi-email</v-icon>
                ing.davidjuarezc@gmail.com
              </div>

              <div class="pt-5 text-body-2 d-flex">
                <v-icon class="pr-3" left small>mdi-map-marker</v-icon>
                <div class="font-weight-bold">
                  <p class="mb-1">Puerto Vallarta, Jalisco</p>
                  <p class="mb-1">Bucerias, Nayarit</p>
                </div>
              </div>

              <div class="pt-5 text-body-2 d-flex">
                <v-icon class="pr-3" left small>mdi-clock-time-nine</v-icon>
                <div class="font-weight-bold">
                  <p class="mb-1">Lun - Vier 10:00 - 19:00</p>
                  <p class="mb-1">Sabado 10:00 - 14:00</p>
                </div>
              </div>
            </div>
            <v-btn
              color="#1D1C1D"
              block
              dark
              tap
              target="_blank"
              class="text-lowercase rounded-0 text-body-2 mb-2 py-3"
              href="https://api.whatsapp.com/send?phone=3221807041&text=Hola!%20"
            >
              <v-icon left small> mdi-whatsapp </v-icon>
              enviar whatsapp
            </v-btn>
            <v-btn
              color="#0072C6"
              block
              class="
                text-lowercase
                white--text
                font-weight-medium
                rounded-0
                text-body-2
                py-3
              "
              href="mailto:misagl@hotmail.com?Subject=Correo%20para%20informacion%20sobre%20Desarrollador%20FullStack"
            >
              <v-icon left small> mdi-email-fast </v-icon>
              enviar correo
            </v-btn>
          </v-form>
        </v-card>
      </transition>

      <v-fab-transition>
        <v-btn
          dark
          absolute
          top
          right
          fab         
          @click="changeIcon"
        >
          <v-icon>{{ icon }}</v-icon>
        </v-btn>
      </v-fab-transition>
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3733.335599716414!2d-105.20879148557007!3d20.655921205778508!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x84214f70b9955c75%3A0x277cb240ac7aaef3!2sBolivia%20548%2C%20Coapinole%2C%2048290%20Puerto%20Vallarta%2C%20Jal.!5e0!3m2!1ses!2smx!4v1656532024461!5m2!1ses!2smx"
        width="100%"
        height="550"
        style="border: 0"
        loading="lazy"
        defer
      >
      </iframe>
    </v-card>
  </v-container>
</template>

<script lang="ts">
export default {
  data: () => ({
    show: true,
    icon: "mdi-eye-remove",
  }),
  methods: {
    changeIcon() {},
  },
};
</script>

<style>
@media (max-width: 600px) {
  .contentForm {
    bottom: 0;
    border-radius: 80px 80px 0px 0px !important;
  }
}

.contentForm {
  position: absolute !important;
  z-index: 1 !important;
  background-color: #f5f5f5 !important;
  widows: 300px !important;
}

.TextWhite {
  color: white !important;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}
</style>