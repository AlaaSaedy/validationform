<template>
  <div id="app">
    <AppHeader />
    <router-view />
    <!--<AppFooter />-->
  </div>
</template>

<script>
import AppHeader from "@/components/global/AppHeader.vue";
//import AppFooter from "@/components/global/AppFooter.vue";
export default {
  name: "App",
  components: {
    AppHeader
    //AppFooter
  }
};
</script>

<style lang="scss">

@import url('https://fonts.googleapis.com/css?family=Baloo+2&display=swap');

#app {
  font-family: 'Baloo 2', cursive;
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
