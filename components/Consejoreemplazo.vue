<template>
  <v-container fluid class="pa-0 ma-0">
    <v-card class="pa-0 ma-0 rounded-0 py-md-10" elevation="0" light max-width="100vw">
      <v-card
        class="pt-10 pb-5 rounded-0 mx-md-auto"
        width="100%"
        max-width="85vw"
        elevation="0"
        light
      >
        <p
          class="
            mb-3
            text-subtitle-2 text-md-h6
            font-weight-black
            text-center text-md-start
            pl-md-0
          "
        >
          ¿No sabes si reemplazar tu aire acondicionado?, Toma estos consejos en
          cuenta.
        </p>
        <v-card
          class="
            rounded-0
            pa-0
            ma-0
            d-flex
            flex-column flex-md-row
            justify-center
            mx-auto
            px-0
            pt-md-6
          "
          elevation="0"
          light
        >
          <nuxt-img
            min-height="150"
            src="/images/reemplazodos.jpg"
            aspect-ratio="1.4"
            loading="lazy"
            sizes="sm:40vw md:50vw lg:30vw"
            class="px-auto"
            format="webp"
            quality="80"
          />
          <v-card class="px-2 pt-8 pt-md-8 rounded-0" elevation="0">
            <div
              class="d-flex pl-md-8 pr-md-15 pb-md-5"
              v-for="(item, i) in consejos"
              :key="i"
            >
              <v-icon color="#EA0A3B" class="pr-4" left
                >mdi-{{ item.icon }}</v-icon
              >
              <p class="text-body-2 pr-md-15 text-md-body-1">
                {{ item.data }}
              </p>
            </div>
          </v-card>
        </v-card>
      </v-card>
    </v-card>
  </v-container>
</template>

<script lang="ts">
export default {
  data() {
    return {
      consejos: [
        {
          data: "Si su aire acondicionado tiene más de 10 años y le da problemas, puede ser en su mejor interés de considerar un reemplazo",
          icon: "alert-circle-check",
        },
        {
          data: "¿Es un nuevo sistema una mejor inversión a largo plazo?Nuestros Ingenieros pueden ayudarle a calcular el retorno de la inversión para determinar si una actualización es más beneficiosa que una reparación.",
          icon: "alert-circle-check",
        },
        {
          data: "Una unidad más eficiente consume menos electricidad y podría ahorrarle mucho en las facturas de energía.",
          icon: "alert-circle-check",
        },
      ],
    };
  },
};
</script>

<style>
</style>