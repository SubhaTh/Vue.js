<template>
    <div class="card">
        <h3> card {{ cardTitle}}</h3>
        <h3>{{ cardBody }}</h3>
    </div>
</template>
<script>
export default {
    name: 'AppCard',
    // props: ['cardTitle', 'cardBody'], instead create an object
    props: {
        // cardTitle: String,
        cardTitle: {
            type: String,
            required: true,
        },
        cardBody: Number,
    }

};
</script>
<style scoped>
h3{
    background-color: aqua;
}
.card{
    height: 100px;
    width: 100px;
    border: 1px solid gray;

}
</style>