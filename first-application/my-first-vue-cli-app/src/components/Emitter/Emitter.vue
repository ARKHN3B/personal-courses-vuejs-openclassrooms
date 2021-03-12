<template>
  <button @click="emitCustomEvent">Emit Event</button>
</template>

<script>
export default {
  name   : "Emitter",
  methods: {
    emitCustomEvent() {
      // 16) Ici, on envoit un événement personnalisé
      this.$emit("custom-event-name", {message: "Mon message personnalisé"});
    }
  }
};
</script>

<style scoped>

</style>