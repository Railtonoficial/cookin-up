<template>
  <Banner />
</template>

<style scoped>

</style>

<script setup>
import { defineComponent } from 'vue';
import Banner from './components/Banner.vue';

defineComponent({
  name: 'App',
  components: {
    Banner
  }
});
</script>