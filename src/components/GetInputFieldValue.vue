<template>
  <div>
    <h1>Get Input Field Value</h1>
    <input type="text" v-model="email" placeholder="Enter email" /><br /><br />
    <input
      type="password"
      v-model="password"
      placeholder="Enter password"
    /><br /><br />
    <button v-on:click="getData()" type="button">Get Values</button>
  </div>
</template>

<script>
export default {
  name: "GetInputFieldValue",
  data() {
    return {
      email: null,
      password: null,
    };
  },
  methods: {
    getData() {
      console.log("values: ", this.email, this.password);
    },
  },
};
</script>

<style>
</style>