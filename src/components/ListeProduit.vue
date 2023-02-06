<template>
  <div>
    <Produit
      v-for="produit in produits"
      :nom="produit.nom"
      :frames="produit.frame"
      :key="produit.nom"
    />
  </div>
</template>

<script>
import Produit from "./Produit.vue";

export default {
  props: ["produits"],
};
</script>

<style lang="scss" rel="stylesheet/scss" scoped>
</style>