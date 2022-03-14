<template>
  <div class="container">
    <header-component title="Task Tracker" />
    <task-component tasks="task -1" isCompleted="false" />
    <task-component tasks='task -2'/>
        <task-component tasks='task -3'/>
            <task-component tasks='and so on ...'/>
    <h5>Copyright(c) 2022 Vishal Ahirwar. All rights reserved india.</h5>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import HomeComponent from './components/Home.vue'
import HeaderComponent from "./components/HeaderComponent.vue";
import TaskComponent from "./components/TaskComponent.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    // HomeComponent
    HeaderComponent,
    TaskComponent,

  },
};
</script>

<style>
.container {
  border-color: rgb(255, 0, 0);
  border-radius: 2px;
  margin: 50px;
  padding: 50px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align:left;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
