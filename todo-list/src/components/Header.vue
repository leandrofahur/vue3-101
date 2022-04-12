<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="Add Task" color="green" @click="onClick()" />
  </header>
</template>

<script>
import Button from "./Button";
export default {
  name: "Header",
  props: {
    title: {
      type: String,
      default: "Task Tracker",
    },
  },
  components: {
    Button,
  },
  methods: {
    onClick() {
      console.log("Clicked!!!");
    },
  },
};
</script>

<style scope>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
