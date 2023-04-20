<template>
  <div>
    <h1>Hello world</h1>
    <!-- <img src="./assets/logo.png" alt=""> -->
    <img src="@/assets/logo.png" alt="">
    <input type="text" v-model="inputValue">
    <h1>{{ inputValue }}</h1>
    <h2 v-if="health === 'bad'">Go to home</h2>
    <h2 v-else-if="health==='ok'">Go to gym</h2>
    <h2 v-else>Go to shopping</h2>
  </div>
</template>
<script>
export default {
  name: 'App',
  data() {
    return {
      inputValue: '',
      health: 'bad',
    };
  }
}
</script>
<style>
</style>