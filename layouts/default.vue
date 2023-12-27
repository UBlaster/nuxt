<template>
  <v-app dark>

    <v-app-bar 
      app 
      height="prominent" 
      dense
      class="px-15" 
      fixed
    >
      <div>
        <v-img src="/logo.png" alt="test"  width="150"  />
      </div>

      <v-spacer />

      <v-btn text>
        <v-icon>mdi-magnify</v-icon>
          <v-text>
            test
          </v-text>
      </v-btn>

      <v-btn text >
        <v-icon>mdi-heart</v-icon>
        <v-text>
          test
        </v-text>
      </v-btn>
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer 
      :absolute="!fixed"
      app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {
      clipped: false,
      drawer: false,
      isMain: true,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
}
</script>


<script scope lang="scss">
.header__main {
  height: 100px;
}
</script>