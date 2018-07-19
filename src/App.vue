<template>
  <div id="app">
    <input type="text" v-model="username" placeholder="Username">
    <input type="text" v-model="repo" placeholder="Repo">
    <branches-selector></branches-selector>
    <commit-list></commit-list>
  </div>
</template>

<script>
import BranchesSelector from "./components/BranchesSelector";
import CommitList from "./components/CommitList";

export default {
  name: "App",
  components: {
    BranchesSelector,
    CommitList
  },
  data() {
    return {
      username: "",
      repo: ""
    };
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
