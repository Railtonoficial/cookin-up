<template>
  <Banner />
  <ConteudoPrincipal />
</template>

<style scoped>

</style>

<script setup>
import { defineComponent } from 'vue';
import Banner from './components/Banner.vue';
import ConteudoPrincipal from './components/ConteudoPrincipal.vue';

defineComponent({
  name: 'App',
  components: {
    Banner,
    ConteudoPrincipal
  }
});
</script>