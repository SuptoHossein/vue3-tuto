<template>
  <div>
    <!-- <h1>Reuse Component</h1> -->
    <!-- <h2>User Component</h2> -->
    <p>{{ usersData.name }}</p>
    <p>{{ usersData.email }}</p>
    <button v-on:click="getAlert(usersData.name)">Alert Name</button>
  </div>
</template>

<script>
export default {
  name: "ReuseComponent",
  props: {
    usersData: Object,
    getAlert: Function,
  },
};
</script>

<style>
</style>