<template>
  <button class="ingrediente" @click="selecionado = !selecionado" :aria-pressed="selecionado">
    <Tag :texto="ingrediente" :ativa="selecionado" />
  </button>
</template>

<script lang="ts">
import Tag from './Tag.vue';

export default {
  name: 'IngredienteSelecionavel',
  components: {
    Tag
  },
  props: {
    ingrediente: {
      type: String,
      required: true,
    },
  },
  data() {
    return {
      selecionado: false,
    };
  },
};
</script>

<style scoped>
.ingrediente {
  cursor: pointer;
}
</style>