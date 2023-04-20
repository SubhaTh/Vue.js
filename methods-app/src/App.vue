<template>
  <div>
    <h1>Hello world</h1>
    <!-- <img src="./assets/logo.png" alt=""> -->
    <img src="@/assets/logo.png" alt="">
    <input type="text" v-model="inputValue">
    <h1>{{ inputValue }}</h1>
  </div>
</template>
<script>
export default {
  name: 'App',
  data() {
    return {
      inputValue: '',
    };
  }
}
</script>
<style>
</style>