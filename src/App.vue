<template>
  <div class="container">
    <header-component title="Task Tracker" />
    <task-component tasks="2hours hv2 Work on miVA " isCompleted="false" />
    <task-component tasks=" Practice on DSA " isCompleted="false" />
    <task-component tasks="C++20 " isCompleted="false" />
    <task-component tasks="C Advanced" isCompleted="false" />
    <task-component tasks="Company Project" isCompleted="false" />
    <task-component tasks="Python3 Django + Vue.js" isCompleted="false" />
    <task-component tasks="C++ B2A" isCompleted="false" />

    <h5>Copyright(c) 2022 \/|eon ENTERPRISES. All rights reserved india.</h5>
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
