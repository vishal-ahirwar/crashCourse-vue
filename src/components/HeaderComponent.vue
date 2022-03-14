<template>
<header>
    <h1>{{title}}</h1>
    <add-task-component/>
    <button-component Action="Add New Task" Color="black" />
</header>
</template>

<script>
import ButtonComponent from './ButtonComponent.vue'
import addTaskComponent from './AddTaskComponent.vue'
export default {
    name:"HeaderComponent",
    props:{
        title:String,
        
    },
    components:{
        ButtonComponent,
        addTaskComponent,
    },
    methods:{
        data(){
            return{taskText:" "}
        }
    }
}
</script>

<style scoped>
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>