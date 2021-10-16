<template>
  <img alt="Vue logo" src="./assets/img/logo.png" />
  <br />
  <router-link to="/">Home</router-link> |
  <router-link to="/About">About</router-link> |
  <router-link to="/Login">Login</router-link>
  <router-view></router-view>
</template>

<script>
// import Home from "@/views/Home.vue";
// import About from "@/views/About.vue";
// import Login from "@/views/Login.vue";

export default {
  name: "App",
  components: {
    // Home: Home,
    // Login: Login,
    // About: About,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}
</style>
