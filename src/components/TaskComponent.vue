<template>
    <h3>{{tasks}}</h3>
</template>

<script>
export default {
    name:'TaskComponent',
    props:{
        tasks:String,
        isCompleted:Boolean,
    }
}
</script>

<style scoped>
h3
{
    padding: 5px;
    margin: 5px;
    border-radius: 5px;
    border-color: blue;
    background-color: #2222;
}
</style>