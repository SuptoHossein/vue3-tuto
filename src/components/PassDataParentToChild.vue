<template>
  <div>
    <h1>Pass data parent to child</h1>
    <h1>{{ name }}</h1>
    <h2>{{ usrDetails.name }}</h2>
    <button v-on:click="usrData()">Click me</button>
  </div>
</template>

<script>
export default {
  name: "PassDataParentToChild",
  props: {
    name: String,
    usrDetails: Object,
    usrData: Function,
  },
};
</script>

<style>
</style>