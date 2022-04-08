<template>
  <div>
    <h1 v-on:mousemove="getConsole()">Vuejs Events</h1>
    <button v-on:click="getData('button 1 click')" type="button">
      Click me</button
    ><br />
    <button v-on:dblclick="getData('button double click')" type="button">
      Click me</button
    ><br /><br /><br />

    <h1>Count: {{ count }}</h1>
    <button v-on:click="decrement()">Decrement</button>
    <button v-on:click="increment()">Increment</button>
  </div>
</template>

<script>
export default {
  name: "EventsComponent",
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    getData(data) {
      alert(data);
    },
    getConsole() {
      console.log("function called");
    },
    decrement() {
      if (this.count > 0) {
        this.count--;
      }
    },
    increment() {
      this.count++;
    },
  },
};
</script>

<style>
</style>