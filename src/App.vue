<template>
   <v-app id="app">
      <v-navigation-drawer
      color="green"
      dark
      expand-on-hover
      hide-overlay
      permanent
      right
      app
      >
        <v-list
            nav 
            shaped
            dense
        >
          <v-list-item>
            <v-list-item-avatar>
              <img :src="'https://randomuser.me/api/portraits/men/27.jpg'">
            </v-list-item-avatar>

            <v-list-item-content class="text-left">

              <v-list-item-title class="font-weight-black">
                  SocialLink
              </v-list-item-title>
              <v-list-item-subtitle>
                Прикольный Парень
              </v-list-item-subtitle>

            </v-list-item-content>
          </v-list-item>

          <v-divider class="my-3"></v-divider>

          <v-list-item link to="/">

            <v-list-item-icon>
              <v-icon>mdi-freebsd</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title class ="text-left">Boss-page</v-list-item-title>
            </v-list-item-content>

          </v-list-item>

          <v-list-item link to="/about">

            <v-list-item-icon>
              <v-icon>mdi-unicorn-variant</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title class ="text-left">Virtual-You</v-list-item-title>
            </v-list-item-content>

          </v-list-item>

          <v-list-item link to="">

            <v-list-item-icon>
              <v-icon>mdi-sunglasses</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title class ="text-left">Virtual-Your-Friends</v-list-item-title>
            </v-list-item-content>

          </v-list-item>

        </v-list>
      </v-navigation-drawer>
    
    <v-content class="px-12 py-3">
      <v-container fluid>
        <router-view/>
      </v-container>
    </v-content>

  </v-app>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
