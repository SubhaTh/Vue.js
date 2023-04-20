<template>
    <div class="card">
        <h1>Count: {{ count }}</h1>
        <button @click="incrementCount">+</button>
        <button @click="decrementCount">-</button>
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
            alert('Count value is: $(this.count)');
        },
        incrementCount() {
            this.count = this.count + 1;
        },
        decrementCount() {
            if (this.count <= 0) {
                alert("Count value can't be zero");
                return;
            }
            this.count = this.count - 1;
        }
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