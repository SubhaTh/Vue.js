<template>
    <div class="card">
        <h1>Count: {{ count }}</h1>
        <button @click="showAlert">+</button>
        <button>-</button>
    </div>
</template>

<script>


export default {
    name: 'AppCard',
    data() {
        return {
            count: 0,
        }
    },
    methods: {
        showAlert() {
            alert('Hi there');
        },
    },
}
</script>


<style scoped>
.card{
    height: 200px;
    width: 300px;
    border: 3px solid gray;
    margin: auto;
    padding : 14px;
    background-color: #fbfbfb
}
button{
    font-size: 20px;
    height: 50px;
    width:100px;
    margin: 2px;
    border:none;
    background-color: green;
    cursor:pointer;
}
</style>