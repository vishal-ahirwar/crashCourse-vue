<template>
    <div>
        <input v-model="taskText" type="text"/>
    </div>
</template>
<script>
export default {
    name:"addTaskComponent",
    methods:{

        data(){
            return {taskText:" "}
        }
    }
}
</script>