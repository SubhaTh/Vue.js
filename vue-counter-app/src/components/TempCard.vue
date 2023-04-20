<template>
    <div class="card" style="max-width: 400px; margin: 15px auto">
        <div class="card-body">
            <p class="card-text">Today's temperature is: {{ celValue }}°C</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'TempCard',
    props: {
        value: {
            type: Number,
            required: true,
        },
    },
    computed: {
        celValue() {
            let cel = [(this.value - 32) * 5] / 9;
            return cel;
        },
    },
};
</script>