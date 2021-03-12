<template>
  <div>
    <h1>{{ title }} #{{ count }}</h1>
    <ul>
      <!-- 12) L'attribut key est fortement utile à l'algorithme de VueJS (Cf. https://v3.vuejs.org/api/special-attributes.html#key) -->
      <li v-for="item in list" :key="item">
        {{ item }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "ItemList",
  props: { // 13) On peut aussi ajouter une vérification des types sur nos props
    list: {
      type: Array,
      default: () => [], // 15) On peut définir une valeur par défaut. Un tableau ou un objet se doit d'être toujours renvoyé par une fonction pour l'argument default.
    },
    title: {
      type: String,
      required: true, // 14) On rend ici la propriété obligatoire
    },
    count: {
      type: Number,
      default: 1,
    }
  }
};
</script>

<style scoped>

</style>