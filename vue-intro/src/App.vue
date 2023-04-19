<template>
    <div>
        <h3 style="color: blue">Hello world</h3>
        <h3 class="greeting">Hii</h3>
        <!-- <app-card v-bind:card-title="3+5"  card-body="Hi there!"></app-card>  -->
        <app-card card-title="one" :card-body="1 +1" card-msg="footer msg" card-type="info"></app-card> 
        <app-card card-title="two" :card-body="2 +5"></app-card>
        <app-card card-title ='three' :card-body="3 +3"></app-card>
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