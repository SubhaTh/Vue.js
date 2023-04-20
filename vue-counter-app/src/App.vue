<template>
  <div>
    
    <app-card title="Counter App"></app-card>
    <app-header></app-header>
  </div>
</template>
<script>
import AppCard from './components/AppCard.vue';
import AppHeader from './components/layout/AppHeader.vue'
export default {
  name: 'App',
  components: { AppCard, AppHeader},
};

</script>

<style>

</style>
