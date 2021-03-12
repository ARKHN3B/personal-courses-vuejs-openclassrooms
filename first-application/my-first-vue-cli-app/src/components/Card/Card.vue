<template>
  <div class="card">
    <!-- 20) Il est possible de nommer ses slots -->
    <slot name="title">Titre de la carte</slot>
    <slot name="text">Texte de la carte</slot>
    <slot name="action">Action</slot>
  </div>
</template>

<script>
export default {
  name: "Card"
};
</script>

<style scoped>

</style>