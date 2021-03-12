<template>
  <!-- 12) Il faut néamoins ajouter l'attribut class avec la directive v-bind -->
  <div v-bind:class="$style.item">Item: {{ $route.params.name }}</div>
</template>

<script>
export default {
  name: "ItemDetail"
};
</script>

<!-- 11) L'attribut module permet - à l'instar de scoped - de délimiter les styles à la portée du composant sans pour
autant être impacté par un style spécifique hérité -->
<style module>
  .item {
    color: red;
  }
</style>