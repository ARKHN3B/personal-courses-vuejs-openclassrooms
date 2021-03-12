<template>
  <a :href="url">{{ text }}</a>
</template>

<script>
export default {
  name: "NavLink",
  props: ["url", "text"], // 05) Voici comment définir des props au niveau d'un composant Vue
};
</script>

<!-- 10) Utiliser l'attribut scoped permet de limiter le bloc de style au composant tout en conservant les styles dits globaux -->
<style scoped>

</style>