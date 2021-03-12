<template>
  <div :class="size">
    <!-- 19) Un slot est un espace ouvert où on peut passer ce que l'on souhaite à l'intérieur à l'image d'un children en React.
             Il est possible de passer une valeur par défaut à notre slot. -->
    <slot>Bonjour ! Voici une valeur par défaut</slot>
  </div>
</template>

<script>
export default {
name: "CustomBanner"
}
</script>

<style scoped>

</style>