<template>
  {{ message }}
<!-- 17) On écoute les événements personnalisés et on assigne une méthode spécifique -->
<!-- 18) Les événements fonctionnent uniquement de l'enfant au parent directement (les composants parents du composant parent ne seront pas impactés) -->
  <Emitter @custom-event-name="setMessage"/>
</template>

<script>
import Emitter from "../Emitter/Emitter";

export default {
  name      : "Listener",
  components: {
    Emitter,
  },
  data() {
    return {
      message: "Hello!",
    };
  },
  methods: {
    setMessage(payload) {
      this.message = payload.message;
    }
  }
};
</script>

<style scoped>

</style>