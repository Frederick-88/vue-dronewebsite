<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <v-btn style="background-color: orange;" large>Large Button</v-btn>
    <v-btn class="ma-2" outlined fab color="teal">
      <v-icon>mdi-format-list-bulleted-square</v-icon>
    </v-btn>
    <div class="text-center">
      <v-rating
        background-color="green lighten-3"
        color="green"
        v-model="rating"
      ></v-rating>
    </div>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
