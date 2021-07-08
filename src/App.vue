<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
    <v-app-bar-nav-icon></v-app-bar-nav-icon>
    <v-toolbar-title>Page Title</v-toolbar-title>
    <v-spacer/>
    <v-btn icon to="/about">
      <v-icon>mdi-magnify</v-icon>
    </v-btn>

    <v-btn icon to="/">
      <v-icon>mdi-magnify</v-icon>
    </v-btn>
    </v-app-bar>

    <v-main>
      <router-view></router-view>
    </v-main>

    <v-footer
      app
      color="primary"
      dark
      absolute
    >
    <v-spacer></v-spacer>
    <div>&copy; {{new Date().getFullYear()}}</div>
    </v-footer>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  })
}
</script>
