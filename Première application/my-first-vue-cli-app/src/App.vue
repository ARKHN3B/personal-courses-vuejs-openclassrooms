<template>
  <div id="app">
    <nav>
      <NavLink url="/" text="Accueil"/>
      <NavLink url="/about" text="À propos"/>
      <NavLink url="/contact" text="Contact"/>
    </nav>
  </div>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import NavLink    from "./components/NavLink/NavLink"; // 05) Import du composant Navlink

export default {
  name      : "App",
  components: {
    HelloWorld,
    NavLink, // 06) Enregitrement du composant via la propriété components,
  }
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
