<template>
  <div>
    <h1>Get Checkbox & Radio Button Value</h1>
    <h3>Technology</h3>
    <label for="java">Java</label>
    <input
      type="checkbox"
      v-model="technology"
      name=""
      value="java"
      id="java"
    />
    <label for="php">PHP</label>
    <input type="checkbox" v-model="technology" name="" value="php" id="php" />
    <label for="node">Node</label>
    <input
      type="checkbox"
      v-model="technology"
      name=""
      value="node"
      id="node"
    />

    <h3>Selected Technology : {{ technology }}</h3>

    <h3>Who I am</h3>
    <label for="student">Student</label>
    <input
      type="radio"
      v-model="identity"
      name="identity"
      value="student"
      id="student"
    />
    <label for="developer">Developer</label>
    <input
      type="radio"
      v-model="identity"
      name="identity"
      value="developer"
      id="developer"
    />

    <h3>I am a : {{ identity }}</h3>
  </div>
</template>

<script>
export default {
  name: "GetCheckbox&RadioButtonValue",
  data() {
    return {
      technology: [],
      identity: [],
    };
  },
};
</script>

<style>
</style>