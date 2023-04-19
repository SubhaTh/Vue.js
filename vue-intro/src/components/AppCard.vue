<template>
    <div class="card">
        <p><small>{{ cardType }}</small></p>
        <h3> card {{ cardTitle}}</h3>
        <h3>{{ cardBody }}</h3>
        <footer>{{ cardMsg }}</footer>
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
        cardMsg: {
            type: String,
            default: function () {
                return 'Footer default props';
            }
        
        },
        cardType: {
            type: String,
            validator: function (value) {
                // return ['sucess', 'error'].includes(value);
                if (value === 'sucess' || value === 'error') {
                    return true;
                }
                return false;
            }

        }
    }

};
</script>
<style scoped>
h3{
    background-color: aqua;
}
.card{
    height: 100px;
    width: 300px;
    border: 1px solid gray;

}
</style>