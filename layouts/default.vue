<template>
  <v-app dark>
    <!--
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      :clipped-left="clipped"
      fixed
      app
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-btn
        icon
        @click.stop="miniVariant = !miniVariant"
      >
        <v-icon>mdi-{{ `chevron-${miniVariant ? 'right' : 'left'}` }}</v-icon>
      </v-btn>
      <v-btn
        icon
        @click.stop="clipped = !clipped"
      >
        <v-icon>mdi-application</v-icon>
      </v-btn>
      <v-btn
        icon
        @click.stop="fixed = !fixed"
      >
        <v-icon>mdi-minus</v-icon>
      </v-btn>
      <v-toolbar-title v-text="title" />
      <v-spacer />
      <v-btn
        icon
        @click.stop="rightDrawer = !rightDrawer"
      >
        <v-icon>mdi-menu</v-icon>
      </v-btn>
    </v-app-bar>

     -->
    
     <v-app-bar app color="#09AEB8" dark elevate-on-scroll dense>
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
      <v-spacer></v-spacer>
      <v-btn href="https://www.facebook.com/optecmantenimiento" target="_blank" text class="ma-0 pa-0" x-small>
        <v-icon left class="ma-0 pa-0">mdi-facebook</v-icon>
      </v-btn>
      <v-btn href="https://api.whatsapp.com/send?phone=3221807041&text=Hola!%20" target="_blank" text class="ma-0 pa-0" x-small >
        <v-icon left class="ma-0 pa-0">mdi-whatsapp</v-icon>
      </v-btn>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" app temporary light>
      <v-card elevation="0" class="text-center" color="transparent" light>
        <v-btn
          height="80"
          elevation="0"
          class="rounded-0 mt-10"
          color="transparent"
          to="/"
          text
        >
          <v-img :src="require(`@/assets/images/icons/OPTEC.svg`)"> </v-img>
        </v-btn>
      </v-card>
      <v-list nav dense class="mt-5">
        <v-list-item-group
          
          active-class="cyan--text text--accent-4 "
        >
          <v-list-item to="/#proyectos" >
            <v-list-item-title
              class="font-weight-light py-6 text-h6 text-center"        
              @click="$vuetify.goTo('#proyectos')"    
               
              >Proyectos</v-list-item-title
            >
          </v-list-item>

          <v-list-item to="/#nosotros">
            <v-list-item-title
              class="font-weight-light py-6 text-h6 text-center"
              @click="$vuetify.goTo('#nosotros')"
              >Nosotros</v-list-item-title
            >
          </v-list-item>

          <v-list-item color="transparent"  to="/#servicios" >
            <v-list-group sub-group no-action class="" >
              <template v-slot:activator>
                <v-list-item-content @click="$vuetify.goTo('#servicios')">
                  <p class="font-weight-light text-h6 pa-0 ma-0">Servicios</p>
                </v-list-item-content>
              </template>
              <v-card elevation="0" class="mt-0" color="transparent">
                <v-list-item
                  v-for="(item, i) in rutas"
                  :key="i"
                  :to="item.ruta"
                  class="ma-0 pa-0"
                >
                  <v-list nav dense class="">
                    <v-list-item-group
                      
                      active-class="black--text"
                    >
                      <v-list-item
                        class="text-body-2 font-weight-normal pa-0 ma-0 px-3 pt-2"
                        :to="item.ruta"
                      >
                        <img
                          width="20"
                          height="20"
                          :src="require(`@/assets/images/icons/${item.icon}`)"
                        />
                        <img />
                        <p class="ma-0 pa-0 pl-5">{{ item.nombre }}</p>
                      </v-list-item>
                    </v-list-item-group>
                  </v-list>
                </v-list-item>
              </v-card>
            </v-list-group>
          </v-list-item>

          <v-list-item>
            <v-list-item-title
              class="font-weight-light py-6 text-h6 text-center"
              @click="$vuetify.goTo('#contacto')"
              to="/#contacto"
              >Contacto</v-list-item-title
            >
          </v-list-item>

          <v-card class="text-center pt-3" elevation="0">
            <v-btn icon class="mx-3" href="https://www.facebook.com/optecmantenimiento" target="_blank">
               <v-icon color="black" class="px-2">mdi-facebook</v-icon>
            </v-btn>
            <v-btn icon class="mx-3" href="https://api.whatsapp.com/send?phone=3221807041&text=Hola!%20" target="_blank">
               <v-icon color="black" class="px-2">mdi-whatsapp</v-icon>
            </v-btn>
            
          </v-card>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
    

    <v-main>
      <v-container fluid class="ma-0 pa-0">
        <btngroup/>
        <Nuxt />
      </v-container>
    </v-main>
    
    <Footer/>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      rutas: [
        {
          nombre: "A/C Instalacion",
          ruta: "/servicios/acinstalacion",
          icon: "AC.svg",
        },
        {
          nombre: "Reemplazo",
          ruta: "/servicios/reemplazo",
          icon: "replaceAC.svg",
        },
        {
          nombre: "Instalaciones electricas en baja tension",
          ruta: "/servicios/bajatencion",
          icon: "bajatension.svg",
        },
        {
          nombre: "AC Reparacion y mantenimiento",
          ruta: "/servicios/acmantenimiento",
          icon: "mainenceAC.svg",
        },
        {
          nombre: "Diagramas y planos electricos",
          ruta: "/servicios/diagramaselectricos",
          icon: "plan.png",
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
