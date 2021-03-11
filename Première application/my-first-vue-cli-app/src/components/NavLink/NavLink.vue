<template>
  <a :href="url">{{ text }}</a>
</template>

<script>
export default {
  name: "NavLink",
  props: ["url", "text"], // 07) Voici comment définir des props au niveau d'un composant Vue
};
</script>

<style scoped>

</style>