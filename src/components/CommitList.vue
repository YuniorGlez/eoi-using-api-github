<template>
  <div class="hello">
    <h1>Hello from commit list component</h1>
    <commit-item v-for="a in 10" :key="a"></commit-item>
  </div>
</template>

<script>
import CommitItem from "./ComitItem";
import axios from 'axios';

export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  },
  components: {
    CommitItem
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
