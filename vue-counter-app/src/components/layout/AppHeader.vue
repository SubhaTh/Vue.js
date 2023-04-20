<template>
    <div>
        <h3 class="app-header">{{ title }}</h3>
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
.app-header{
    margin-top:0;
    text-align: center;
    padding: 4px;
}

</style>