<template>
  <div>
    <h1 v-if="show">If Condition</h1>
    <!-- <h1 v-else>Else Condition</h1> -->
    <button v-on:click="toggle()">Show</button>
  </div>
</template>

<script>
export default {
  name: "IfElse",
  data() {
    return {
      show: true,
    };
  },
  methods: {
    toggle() {
      this.show = !this.show;
    },
  },
};
</script>

<style>
</style>