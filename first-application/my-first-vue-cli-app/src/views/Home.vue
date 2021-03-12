<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Listener/>
    <!-- 21) Voici comment attribuer plusieurs slots -->
    <Card>
      <template v-slot:title>
        <h3>Donner des noms aux slots est utile</h3>
      </template>
      <template v-slot:text>
        <p>Maintenant, on peut ajouter ce que l'on veut ici en donnant le nom du slot !</p>
      </template>
      <template v-slot:action>
        <a href="#">En savoir plus</a>
      </template>
    </Card>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import Listener   from "../components/Listener/Listener";
import Card       from "../components/Card/Card";

export default {
  name      : "Home",
  components: {
    HelloWorld,
    Listener,
    Card,
  }
};
</script>
