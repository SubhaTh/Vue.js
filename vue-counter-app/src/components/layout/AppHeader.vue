<template>
    <div>
        <h3>{{ title }}</h3>
    </div>

</template>
    
<script>
export default {
    name: 'AppHeader',
    props: {
        title: {
            type: String,
            required: true,
            default: function () {
                return 'App Title'
            },
        },
    },
};
</script>
<style scoped>
header{
    background-color : gray;
}

</style>