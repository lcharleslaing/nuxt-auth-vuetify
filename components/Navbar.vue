<template>
<v-container fluid
    class="mx-auto overflow-hidden"
    height="100vh"
  >
    <v-app-bar app
      color="primary"
    >
      <v-app-bar-nav-icon @click="drawer = true" />

      <v-toolbar-title>Big2Tiny</v-toolbar-title>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
      height="100vh"
    >
      <v-list
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Account</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </v-container></template>
<script>
  export default {
    data: () => ({
      drawer: false,
      group: null,
    }),
  }
</script>

<style lang="sass" scoped>

</style>

