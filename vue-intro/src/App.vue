<template>
    <div>
        <h3 style="color: blue">Hello world</h3>
        <h3 class="greeting">Hii</h3>
        <app-card></app-card>
    </div>
</template>
<script>
import AppCard from './components/AppCard.vue';
export default {
    name: 'App',
    components: { AppCard },
};
</script>
<style>
.greeting{
    color:pink;
}
</style>