<template>
    <button v-on:click="onClick" v-bind:style="{background:Color}">{{Action}}</button>
</template>

<script>
export default {
    name:"ButtonComponent",
    props:{
        Action:String,
        Color:String,
    },
    methods:
    {

        onClick()
        {
            alert("Would you like to add new task")
        }
    }
}
</script>
<style scoped>
    button{
        margin: 15px;
        padding: 15px;
        padding-left: 35px;
        padding-right: 35px;
        border-color: rgb(26, 21, 21);
        color: white;
    }
</style>