<template>
  <div>
    <h1>Methods and params</h1>
    <p>{{ getName("Peter") }}</p>
    <p>{{ getName("brouce") }}</p>
    <p>{{ getData().email }}</p>
  </div>
</template>

<script>
export default {
  name: "MethodsWithParams",
  data() {
    return {
      email: "supto.hossein@gmail.com",
    };
  },
  methods: {
    getName(name) {
      return name;
    },
    getData() {
      return {
        name: "supto",
        email: this.email,
      };
    },
  },
};
</script>

<style>
</style>``