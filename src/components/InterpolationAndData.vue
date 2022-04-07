<template>
  <div>
    <h1>InterpolationAndData {{ "Hello".length }}</h1>
    <h1>Email: {{ email }}</h1>
    <p>Mobile: 0{{ mobile }}</p>
    <p>Mobile: 0{{ (mobile = 8888) }}</p>
    <p>{{ getName("supto hossein") }}</p>
  </div>
</template>

<script>
export default {
  name: "InterpolationAndData",
  data() {
    return {
      email: "supto.hossein@gmail.com",
      mobile: 1738245153,
      getName: function (a) {
        return a;
      },
    };
  },
};
</script>

<style>
</style>