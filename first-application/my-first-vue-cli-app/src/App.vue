<template>
  <div id="nav">
    <router-link to="/">Home</router-link>
    |
    <router-link to="/about">About</router-link>
    |
    <!-- 07) Voici un lien de type routeur -->
    <router-link to="/item/croissant">Croissant</router-link>
  </div>
  <!-- 06) Voici le routeur et les composants associés qui seront rendus à l'intérieur -->
  <router-view/>
</template>

<script>
// 08) Il est possible d'utiliser des hooks de cycle de vie en passant certaines fonctions spécifiques à VueJS
// Cf. https://v3.vuejs.org/guide/instance.html#lifecycle-diagram
export default {
  beforeCreate() { console.log("Je ne suis pas encore créé") },
  created() { console.log("Je suis créé") },
  beforeMount() { console.log("Je vais bientôt être monté sur le DOM") },
  mounted() { console.log("Je suis monté sur le DOM") },
};
</script>

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
